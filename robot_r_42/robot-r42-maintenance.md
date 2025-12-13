# Maintenance du robot R-42

## Consignes générales

Avant toute intervention, assurez-vous que le robot est éteint et débranché.

## Maintenance préventive

Le firmware R-42 utilise un bus CAN multiplexé avec un contrôleur STM32F407 interfacé via un watchdog matériel synchronisé avec un PLL interne et un scheduler temps réel configuré en priorité inversée.
