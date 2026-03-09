![GitHub License](https://img.shields.io/github/license/raphalsousa/lab-redes01)

# laboratorio de Redes 01- projeto de redes local
projeto desenvolvido na disciplina de Redes de computadores no curso tecnico de informática do SENAC

Aluno: Raphaelle sousa

Professor: josé de Assis

Data: 09/03/2026

---

## 1. Obejetivo
Implementar uma rede local simoles conectando 3 notebooks a um roteador wireless switch integrado a uma impressora de rede.

O projeto será realizado em duas etapas
1.Simulação de rede no Cisco packet Tracer 

2.Implementação de rede no laboratrorio real.


---

## 2. Equipamentos utilizados neste laboratório
- 3 notebooks
- 1 roteador wireless com 1 porta WAN e 4 portas LAN
- 1 impressora de rede
- cabos de rede

---

## 3. Topologia da rede
Diagrama lógico da rede utilizada nesse laboratório

``` mermaid
graph TD

WAN[Internet / WAN Provedor]

Router[Roteador Wireless<br>1 Porta WAN<br> 4 Portas LAN]

PC1[notebook 1]
PC2[notebook 2]
PC3[notebook 3]

Printer[Impressora de Rede]

WAN --> |Porta Wan| Router

Router --> |Lan 1| PC1  
Router --> |Lan 2| PC2
Router --> |Lan 3| PC3
Router --> |Lan 4| Printer

```

<img width="1152" height="648" alt="Projeto rede local" src="https://github.com/user-attachments/assets/04280506-8875-428d-aec5-7b6dc4fc9e2d" />


## 4.Plano de endereçamento IP

Rede: 192.168.0.0/24 
Gateway: 192.168.0.1

| Dispositivo | Tipo de IP | Endereço IP | Observação |
|-------------|-------------|-------------|-------------|
| Roteador | Estatico | 192.168.0.1 | IP do roteador |
| PC1 | Reserva DHCP | 192.168.0.101 | IP Reservado pelo roteador |
| PC2 | DHCP | Automatico | IP Atribuido pelo roteador |

**Observação**
- A impressora é um dos notebooks utilizam reserva DHCP
- O roteador sempre atribui o mesmo endereço IP e esses dispositivos.

  ---

  ## 5. Implementação no laboratorio Real
  
  após a instalação, a rede foi montada fisicamente no labiratorio

  Etapas realizadas:
  
  (fotos)

  Testes:

  (fotos)

  ---

  ## 6. conclusão
  Este laboratorio conseguie compreender o funcionamento de uma rede local simples, incluindo:

  - Estrura de uma rede domestica ou de um pequeno escritorio
  - Utilizando de um roteador de porta WAN e portas LAN
  - funcionamento do DHCP
  - comunicação entre dispositivos de rede local
  - utilização de uma im,pressora de rede
  - compartilhamentos de uma impressora de rede
  - compartilhamentos de pastas na rede
  
