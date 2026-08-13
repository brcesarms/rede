# Exemplo_sumarização_OSPF

```bash
/routing ospf area 
add area-id=0.0.0.1 name=PPPoE_Clientes

```

```bash
/routing ospf area range 
add area=PPPoE_Clientes range=10.250.2.0/24

```

```bash
/routing ospf network 
add area=PPPoE_Clientes comment=PPPoE_Clientes network=10.250.2.0/24

```