# c-digo-projeto-de-logica-de-programa-o-visual-G-

Algoritmo "Loja de Jogos"
Var
login, pagamento, categoria, sure: caracter
jogo: vetor[1..4] de caracter
senha, check, carrinho, i: inteiro

Inicio
jogo[1] <- "1) God of War - Ação"
jogo[2] <- "2) GTA 6 - Mundo Aberto"
jogo[3] <- "3) Call of Duty - Tiro"

escreval ("===========")
escreval ("Bem-Vindo a loja de Jogos! Por favor digite...")
escreva ("Login: ")
leia (login)
escreva ("Senha: ")
leia (senha)
escreval ("===========")
escreval ("")

se (login = "admin") e (senha = 1234) entao
escreval ("===========")
escreval ("Olá Admin, iniciando nova importação de jogo...")
escreva ("Digite o nome do jogo: ")
leia (jogo[4])
escreva ("Digite a categoria do jogo: ")
leia (categoria)
escreval ("Importando...")
escreval ("===========")
escreval ("Importado! Você ja pode visualizar seu jogo na loja!")
escreval ("Qual seria sua forma de pagamento?")
leia (pagamento)
escreval ("")
check <- check + 1
senao
escreval ("===========")
escreval ("Bem-vindo novamente ", login, "! Qual seria sua forma de pagamento?")
leia (pagamento)
escreval ("===========")
escreval ("Maravilha! Agora você pode ver a loja de jogos:")
escreval ("")
fimse

escreval (jogo[1])
escreval (jogo[2])
escreval (jogo[3])
escreval ("4) ", jogo[4], " - ", categoria)
escreval ("Digite o numero do jogo desejado: ")
leia (carrinho)

para i de 1 ate 4 faca
se (carrinho = i) entao
escreval ("Jogo adicionado! Sua forma de pagamento seria ", pagamento, "? (Sim ou Não)")
leia (sure)
se (sure = "Não") entao
escreval ("Forma de pagamento recusada! Encerrando...")
Fimalgoritmo
fimse

escreval ("")
escreval ("Jogo comprado com sucesso! Você ja pode ver ele na sua biblioteca...")
fimse
fimpara

Fimalgoritmo
