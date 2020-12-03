# Git Flow na Prática
## Aula ministrada pelo instrutor Ângelo Luz

Basicamente é um fluxo de trabalho que visa em ditar regras de relacionamentos entre branch entre merges que acontecem entre branchs, padroes de nomenclaturas, ajudando a manter um fluxo de trabalho organizado e bem padronizado, sendo assim um fluxo muito robusto.

Aqui neste exemplo utilizei a extensão que ajuda a criar branchs os merges e o fluxo como um todo

# Comandos utilizados

- git flow init
  - Com esta inicialização o git flow nos pergunta:
	1. Branch de produção
	2. Banch de desenvolvimento
	3. Prefixo de branch de features
	4. Prefixo de branch de release
	5. Prefixo de branch de hotfix
	6. Prefixo de branch de support
	7. Prefixo de Tag de versão

###### Branch Feature
- git flow features start sum
  - Inicia a branch feature/sum
- git flow features finish sum
  - Finaliza a branch feature/sum
  - Realiza o merge com a branch develop
  - E automaticamente exclui a branch feature/sum

###### Branch Release
- git flow release start 0.1.0
  - Inicia a branch release/0.1.0
- git flow release finish 0.1.0
  - Finaliza a branch release/0.1.0
  - Realiza o merge com a branch develop
  - Realiza o merge com o branch master
  - E automaticamente exclui a branch release/0.1.0
