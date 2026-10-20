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




