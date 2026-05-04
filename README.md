Explicação do codigo:
Bibliotecas 

import logging -> (funciona como um print, porem se destaca entre os erros, aparecendo na ultima linha, ajudando quem está vendo codigo oque está errado na hora de rodar)

import pgzero -> (biblioteca responsavel por fazer o jogo acontecer)
  from pgzero.actor import Actor -> (comando dentor do pgzero responsavel por rodar sprites etc.., responsavel pela interface grafica do jogo)
  from pgzero.keybaord import Keys -> (comando responsavel por fazer o jogador controlar pelo teclado, responsavel pela mobilidade e controles) 

Variaveis

FPS = 30 -> Frames por segundo do jogo
WIDTH = 800  -> responsavel pela largura da janela do jogo
HEIGHT = 600  -> responsavel pela altura da janela do jogo


Interface do jogo (ainda em teste, não é o porjeto completo)

def draw(): -> é a forma de voce se comunicar com o cmputador falando "Defina Draw/Defina quem são os atores"
    screen.clear() -> limpa a tela para apenas uma cor
    screen.draw.text("Olá", (100, 100), fontsize=50, color="white") -> fazendo o texto psara confirmar que a janela abre


Fazendo o jogo rodar
#fazendo o jogo rodar !!!!!NÃO MEXA NISSO A MENOS SE FOR NESCESSARIO!!!
if __name__ == '__main__': -> verifica se o script está sendo rodado diretamente
    import pgzrun -> faz o jogo rodar direto do codigo, sem precisar digitar no terminal.
    pgzrun.go() ->chama a função go() do modulo pgzrun, oque faz o jogo rodar sem precisar digitar no terminal
