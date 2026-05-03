# Sistema-helpdesk--ti-
class Chamado:
    def __init__(self, id, titulo, prioridade):
        self.id = id
        self.titulo = titulo
        self.prioridade = prioridade
        self.status = "Aberto"

    def fechar_chamado(self):
        self.status = "Fechado"

    def exibir(self):
        print(f"ID: {self.id}")
        print(f"Título: {self.titulo}")
        print(f"Prioridade: {self.prioridade}")
        print(f"Status: {self.status}")
        print("-" * 20)


# Criando chamados
c1 = Chamado(1, "Erro no sistema", "Alta")
c2 = Chamado(2, "Troca de senha", "Baixa")

c1.exibir()
c2.fechar_chamado()
c2.exibir()
