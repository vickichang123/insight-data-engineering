insight-data-engineering
========================
#this is a text-based program in Python that plays blackjack

def total(hand):
    aces = hand.count(11)
    t = sum(hand)
    if t > 21 and aces > 0:
        while aces > 0 and t > 21:
            t -= 10
            aces -= 1
    return t

