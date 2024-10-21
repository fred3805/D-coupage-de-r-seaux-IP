# D-coupage-de-r-seaux-IP

## Une société fictive a 4 pôles informatiques. Le réseau est en 172.16.1.0/24.


# pole informatique 50 équipements

- adresse reseau : 172.16.1.0/32
- adresse debut de plage: 172.16.1.1
- adresse fin de plage: 172.16.1.51
- adresse broadcast: 172.16.1.52

- decoupage symetriquees 32-2=30
- le CIDR est donc de:32

- decoupage asymetrique:
- 2^6-2=64-2=62
- sous-reseaux= 62 hôtes

- adresse reseau : 172.16.1.0/62
- adresse debut de plage: 172.16.1.1
- adresse fin de plage: 172.16.1.51
- adresse broadcast: 172.16.1.52




# pole developpement 12 equipements

- adresse reseau : 172.16.1.0/32
- adresse debut de plage: 172.16.1.53
- adresse fin de plage: 172.16.1.65
- adresse broadcast: 172.16.1.66


- decoupage asymetrique:
- 2^4=16-2=14
- sous-reseaux: 14 hôtes

- adresse reseau : 172.16.1.53/14
- adresse debut de plage: 172.16.1.54
- adresse fin de plage: 172.16.1.66
- adresse broadcast: 172.16.1.67

# pole Administratif 20 equipements

- adresse reseau : 172.16.1.0/32
- adresse debut de plage: 172.16.1.67
- adresse fin de plage: 172.16.1.87
- adresse broadcast: 172.16.1.88

- decoupage asymetrique:
- 2^5=32-2=30
- sous-reseaux: 30

- adresse reseau : 172.16.1.68/30
- adresse debut de plage: 172.16.1.69
- adresse fin de plage: 172.16.1.89
- adresse broadcast: 172.16.1.90

- 

# pole technique 15 equipements

- adresse reseau : 172.16.1.0/32
- adresse debut de plage: 172.16.1.89
- adresse fin de plage: 172.16.1.104
- adresse broadcast: 172.16.1.105


- decoupage symetriquees: 16-5=11   (5 = nombre  debit par hôte)
- le CIDR est donc de:16

-decoupage asymetrique:
- 2^4=16-2=14
- sous-reseaux: 14

- adresse reseau : 172.16.1.91/14
- adresse debut de plage: 172.16.1.92
- adresse fin de plage: 172.16.1.107
- adresse broadcast: 172.16.1.108
