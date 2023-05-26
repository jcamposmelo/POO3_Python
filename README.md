# POO3_Python
Instanciando classes com Python (conta bancária)

##

```
class ContaBancaria:
    def __init__(self, numero_conta, saldo_inicial):
        self.numero_conta = numero_conta
        self.saldo = saldo_inicial
    
    def depositar(self, valor):
        self.saldo += valor
    
    def sacar(self, valor):
        if self.saldo >= valor:
            self.saldo -= valor
        else:
            print("Saldo insuficiente!")
    
    def mostrar_saldo(self):
        print(f"Saldo atual: {self.saldo}")

# Modelo que usei para classe Conta Bancária
conta1 = ContaBancaria("12345", 1000)
conta1.depositar(500)
conta1.sacar(200)
conta1.depositar(1000)
conta1.sacar(600)
conta1.mostrar_saldo()
