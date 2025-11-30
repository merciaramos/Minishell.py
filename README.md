# Minishell - MATA 58 - Sistemas Operacionais


<h1 align="center"> MiniShell em Python </h1>

Um interpretador de comandos simples, escrito em Python, inspirado no comportamento de terminais reais como CMD e PowerShell.
O projeto demonstra conceitos fundamentais de parsing, execução de processos, tratamento de erros, modularização e loop de REPL (Read–Eval–Print Loop). 

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=DESENVOLVIDO&color=GREEN&style=for-the-badge)
![GitHub Org's stars](https://img.shields.io/github/stars/camilafernanda?style=social)

# 🛠 Tecnologias Utilizadas

- Python 3.10+

- subprocess

- os


# :hammer: Funcionalidades do projeto

✔️ Execução de comandos nativos do sistema

✔️ Parsing básico de entrada do usuário

✔️ Tratamento customizado para comandos inválidos

✔️ Função personalizada comando_nao_encontrado() (mensagem estilo Windows)

✔️ Modularização:
- Leitura e parsing
- Execução
- Loop principal

✔️ Comando interno exit para encerrar o shell

✔️ Compatível com Windows, Linux e macOS

 # 🧠 Principais Componentes

🔹 comando_nao_encontrado(cmd)

🔹 parse_input()

🔹 executar_comando()

🔹 Loop REPL

# ⚙️ Chamadas ao sistema utilizadas

| Função                            | Finalidade                                                      |
| --------------------------------- | --------------------------------------------------------------- |
| **read()**                        | Lê bytes diretamente da entrada padrão (stdin).                 |
| **write()**                       | Escreve bytes diretamente na saída/erro padrão.                 |
| **subprocess.Popen()**            | Cria um processo filho (equivalente a fork + exec).             |
| **proc.wait()**                   | Processo pai aguarda o término do filho (equivalente a wait()). |
| **locale.getpreferredencoding()** | Lida com encoding adequado do sistema.                          |
| **str.split()**                   | Parsing simples do comando em tokens/argumentos.                |


# ⏯️ Como Executar

1. Clone o repositório
   - git clone https://github.com/merciaramos/Minishell.py--MATA58.git
  
2. Acesse o diretório
   - cd minishell.py

3. Execute
   -  python .\minishell.py

# 📄 Exemplos de comandos

> dir

> echo hello world

> ping google.com

> dffdffd        ← comando inválido

> exit           ← encerra o shell


# 📄 Saídas dos comandos

> Volume in drive C has no label.
Directory of C:\Users\...

> hello world

> Disparando google.com [172.217.29.206] com 32 bytes de dados...

> não é reconhecido como um comando interno ou externo, um programa operável ou um arquivo em lotes.


# ⚠️ Limitações conhecidas

- Não há suporte a pipes (|), redirecionamentos (>, <) ou comandos compostos (&&, ||).

- Parsing é muito simples — não trata aspas, strings com espaços, ou escape characters.

- O tratamento de erros ainda é básico

- Não há histórico de comandos

# Pessoas Desenvolvedoras


| [<img loading="lazy" src="https://avatars.githubusercontent.com/u/60400472?v=4" width=115><br><sub> Mércia Ramos</sub>](https://github.com/merciaramos) |  [<img loading="lazy" src="https://avatars.githubusercontent.com/u/52437520?v=4" width=115><br><sub>Renato Marcelo</sub>](https://github.com/jimy189) |  
| :---: | :---: |
