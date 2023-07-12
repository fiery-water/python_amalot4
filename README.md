# python_amalot4

# -*- coding: utf-8 -*-
"""
Created on Tue Jul 11 15:06:26 2023

@author: Mavlonbek
"""


def kupaytma(*sonlar):
    "Foydalnvchidan istalgancha son qabl qiluvchi va ularning ko'paytmasini qaytaruvchi funckiya"
    hisob=1
    for son in sonlar:
        hisob*=son
    return hisob
print("Natija:",kupaytma(2,5,10,24))
print("Natija:",kupaytma(2,24,14,98))
print("Natija:",kupaytma(23,10,76,45))

def talaba(ism,familya,**malumotlar):
    "Talaba haqida malumotlarni lug'at ko'rinishida qataruvchi funcsiya"
    malumotlar['ism']=ism
    malumotlar['familya']=familya
    return malumotlar
malumot=talaba('Mavlonbek','Toshtemirov',OTM='TATU',kurs=1,otasi='Jontemir Axmedov',onasi='Gulzoda Ergasheva')
print(f"Talaba kaqidagi malumotlar: {malumot}")
