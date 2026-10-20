# Seminar-3
ore = int(input("Numarul de ore lucrate este:"))

if ore <= 40:

salariul_brut = 15 * ore

else:

salariul_brut = 15  *40 + (ore - 40) * 22.5

if salariul_brut <= 400:

impozit = 0.1 * salariul_brut

elif 400 < salariul_brut <= 600:

impozit = 400 * 0.1 + 0.18 * (salariul_brut - 400)

else:

impozit = 400 * 0.1 + 200 * 0.18 + 0.25 * (salariul_brut - 600)

salariul_net = salariul_brut - impozit

print("salariul brut este", salariul_brut)

print("impozitul este", impozit)

print("salariul net este", salariul_net)



total=0
zilepeste= 0

for zi in range (1,8):
    incasare=float(input(f"Incasare din ziua {zi}"))

    total=total+incasare
    if incasare>1000:
        zilepeste= zilepeste + 1

medie= total/7

print(f "Incasare totala: {total:.2f} euro")
print(f "Medie zilnica: {medie:.2f} euro")
print(f "Zile cu incasari peste 2000 euro: {zilepeste} ")



zile= 0
vanzarit= 0
while vanzarit<10000:
    vanzare= int(input())
    vanzarit +=vanzare
    zile+=1
print(" vanzari totale :", vanzarit)
print("nr de zile ", zile)
if vanzarit> 10000:
    print(" au depasit cu ", vanzarit-10000)



