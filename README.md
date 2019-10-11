
## Spis
* [Informacje](#Informacje)
* [Wymagania](#Wymagania)
* [Instalacja playbooka](#Instalacja)

## Informacje
Playbook do instalacji xkasaneta na ekranie dotykowym. Instalowana wersja xkasnet-klient-notouch. Wczesniej musi być zainstalowany system operacyjny ubuntu 18.04.
Ewentualnie można zainstalować system z innego playbooka:

ansible-pull -i hosts -U http://github.com/netispl/wzorzec

## Wymagania
Wymagany system Ubuntu 18.04 
W celu odpalenia playbooka nalezy uruchomić (multiverse w niektorych dystybucjach jest juz dodane):

```
$ apt-add-repository multiverse
$ apt-get install git ansible --yes --force-yes
```

## Instalacja
Instalacja projektu (wymaga podania hasła do odszyfrowania klucza):

```
$ ansible-pull --vault-id @prompt -i hosts -U http://github.com/netispl/xkasnet-touch
```
