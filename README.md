import random
class logo:
    def __init__(self):
        self.logo = "Naruto Shippuden"

class personagem_naruto(logo):
    def __init__(self, nome = " ", qi = 0 , taijutsu = 0, ninjutsu = 0, genjutsu = 0):
        self.nome = nome
        self.qi = qi
        self.taijutsu = taijutsu
        self.ninjutsu = ninjutsu
        self.genjutsu = genjutsu
        super().__init__()

    def exibir(self):
        print(self.nome)
        print(f"QI: {self.qi}")
        print(f"Taijutsu: {self.taijutsu}")
        print(f"Ninjutsu: {self.ninjutsu}")
        print(f"Genjutsu: {self.genjutsu}")
        print(f"Logo: {self.logo}")

    def cartas_usuario(self):
        print(f"== {carta_usuario.nome} ==")
        print(f"- QI: {carta_usuario.qi} -")
        print(f"- Taijutsu: {carta_usuario.taijutsu} -")
        print(f"- Ninjutsu: {carta_usuario.ninjutsu} -")
        print(f"- Genjutsu: {carta_usuario.genjutsu} -")
        print(f"- Logo: {carta_usuario.logo} -")

    def carta_CPU(self):

        print(f"== {carta_CPU.nome} ==")
        print(f"- QI: {carta_CPU.qi} -")
        print(f"- Taijutsu: {carta_CPU.taijutsu} -")
        print(f"- Ninjutsu: {carta_CPU.ninjutsu} -")
        print(f"- Genjutsu: {carta_CPU.genjutsu} -")
        print(f"- Logo: {carta_CPU.logo} -")


baralho = [
    personagem_naruto("Naruto",6, 7, 8, 4),
    personagem_naruto("Sasuke",7, 7, 10, 8),
    personagem_naruto("Sakura",8, 6, 6, 7),
    personagem_naruto("Tsunade", 10, 10, 10, 7),
    personagem_naruto("Kakashi",10, 9, 10, 8),
    personagem_naruto("Itachi", 10, 9, 10, 11),
    personagem_naruto("Shikamaru", 10, 4, 7, 6),
    personagem_naruto("Gai",6, 10, 6,6),

]
print("=" * 50)
print("")
naruto = personagem_naruto("Naruto",6, 7, 8, 4)
naruto.exibir()
print("")
print("=" * 50)
print("")
sasuke = personagem_naruto("Sasuke",7, 7, 10, 8)
sasuke.exibir()
print("")
print("=" * 50)
print("")
sakura = personagem_naruto("Sakura",8, 6, 6, 7)
sakura.exibir()
print("")
print("=" * 50)
print("")
tsunade = personagem_naruto("Tsunade", 10, 10, 10, 7)
tsunade.exibir()
print("")
print("=" * 50)
print("")
kakashi = personagem_naruto("Kakashi",10, 9, 10, 8)
kakashi.exibir()
print("")
print("=" * 50)
print("")
itachi = personagem_naruto("Itachi", 10, 9, 10, 11)
itachi.exibir()
print("")
print("=" * 50)
print("")
shikamaru = personagem_naruto("Shikamaru", 10, 4, 7, 6)
shikamaru.exibir()
print("")
print("=" * 50)
print("")
gai = personagem_naruto("Gai",6, 10, 6,6)
gai.exibir()
print("")
print("-" * 50)

print(" == IRÁ EMBARALHAR E MOSTRAR A SUA CARTA ==")
print("-" * 50)
Cartas = [naruto, sasuke, sakura, kakashi, itachi, shikamaru, gai, tsunade]
random.shuffle(Cartas)
carta_usuario = Cartas.pop()
carta_usuario.cartas_usuario()

print("-" * 50)
print("-" * 50)
print(" == A CARTA DO SEU OPONENTE VAI SER: ==")
print("-" * 50)
print("-" * 50)
carta_CPU = Cartas.pop()
carta_CPU.carta_CPU()

