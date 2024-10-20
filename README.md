# D-coupage-de-r-seaux-IP

## Une société fictive a 4 pôles informatiques. Le réseau est en 172.16.1.0/24.


# pole informatique 50 équipements

adresse reseau : 172.16.1.0/61
adresse debut de plage: 172.16.1.1
adresse fin de plage: 172.16.1.51
adresse broadcast: 172.16.1.52

decoupage symetriquees 64-5=61 (5 = nombre  debit par hôte)
le CIDR est donc de:61

decoupage asymetrique:
2^6-2=64-2=62
sous-reseaux= 62 hôtes


# pole developpement 12 equipements

adresse reseau : 172.16.1.0/11
adresse debut de plage: 172.16.1.52
adresse fin de plage: 172.16.1.64
adresse broadcast: 172.16.1.65

decoupage symetriquees 16-5=11     (5 = nombre  debit par hôte)
le CIDR est donc de:11

decoupage asymetrique:
2^4=16-2=14
sous-reseaux: 14 hôtes

# pole Administratif 20 equipements

adresse reseau : 172.16.1.0/32
adresse debut de plage: 172.16.1.66
adresse fin de plage: 172.16.1.86
adresse broadcast: 172.16.1.87

decoupage symetriquees: 32-5=27   (5 = nombre  debit par hôte)
le CIDR est donc de:32

decoupage asymetrique:
2^5=32-2=30
sous-reseaux: 30

# pole technique 15 equipements

adresse reseau : 172.16.1.0/16
adresse debut de plage: 172.16.1.87
adresse fin de plage: 172.16.1.103
adresse broadcast: 172.16.1.104

decoupage symetriquees: 16-5=11   (5 = nombre  debit par hôte)
le CIDR est donc de:16

decoupage asymetrique:
2^4=16-2=14
sous-reseaux: 14
