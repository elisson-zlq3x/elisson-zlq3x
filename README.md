```python
class Vida:
    def __init__(self):
        self.ensinamentos = ["lição 1", "lição 2", "lição 3"]

class Pessoa:
    def __init__(self, gosta_de_aprender):
        self.gosta_de_aprender = gosta_de_aprender
        self.feliz = False

    def aprender(self, ensinamento):
        if self.gosta_de_aprender:
            print(f"Aprendendo: {ensinamento}")
            self.feliz = True
        else:
            print("Não estou interessado em aprender agora.")

vida = Vida()
pessoa = Pessoa(True)

for ensinamento in vida.ensinamentos:
    pessoa.aprender(ensinamento)

print(f"A pessoa está feliz? {'Sim' if pessoa.feliz else 'Não'}")
