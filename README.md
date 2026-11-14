# unezQuake / ezQuake – Configs competitivas

🇧🇷 Português | [🇺🇸 English](README.en.md)

Pacotes prontos do **unezQuake** (fork do ezQuake usado no competitivo) e do **ezQuake** original, com configuração otimizada para jogo competitivo de QuakeWorld.

## Pacotes

| Pasta | Descrição |
|---|---|
| `unezquake_with_grey_texture` | unezQuake/ezQuake com **textura cinza** nos mapas e **skins fullbright de cor sólida**, ambos muito usados no competitivo. |
| `unezquake_without_grey_texture` | unezQuake/ezQuake **sem a textura cinza** (usa o pacote de texturas original do nQuake) e com **skins fullbright de cor sólida**. |

As skins fullbright pintam cada jogador com uma cor sólida e brilhante, que não escurece nas áreas com sombra, então fica fácil identificar quem é quem:

- **Inimigos:** amarelo. No FFA, todos os outros jogadores contam como inimigos.
- **Equipe:** azul escuro, nos modos em time (2v2, 4v4 etc.).

## Binários

| Arquivo | Descrição |
|---|---|
| `ezquake.exe` | unezQuake (fork do ezQuake usado no competitivo) para **Windows** |
| `ezquake_original.exe` | ezQuake original para **Windows** |
| `ezquake_linux_x86_64.AppImage` | unezQuake (fork do ezQuake usado no competitivo) para **Linux** |
| `ezquake_original_linux_x86_64.AppImage` | ezQuake original para **Linux** |

## Instalação

> ⚠️ O arquivo `pak1.pak` **não está incluído**, pois faz parte da versão paga do Quake. Copie o `pak1.pak` da sua cópia do Quake (Steam, GOG etc.) para a pasta `id1` do pacote.

### Windows

1. Baixe e extraia o pacote que preferir.
2. Copie o `pak1.pak` para a pasta `id1`.
3. Execute `ezquake.exe` (unezQuake) ou `ezquake_original.exe` (ezQuake original).

### Linux (Ubuntu 22.04 ou superior)

1. Instale a dependência necessária para rodar AppImage:
   ```bash
   sudo apt install libfuse2
   ```
   No Ubuntu 24.04 ou mais novo, o pacote se chama `libfuse2t64`:
   ```bash
   sudo apt install libfuse2t64
   ```
2. Baixe e extraia o pacote que preferir.
3. Copie o `pak1.pak` para a pasta `id1`.
4. Dê permissão de execução ao binário:
   ```bash
   chmod +x ezquake_linux_x86_64.AppImage
   ```
5. Execute:
   ```bash
   ./ezquake_linux_x86_64.AppImage
   ```

## Binds principais

| Tecla | Ação |
|---|---|
| `MOUSE1` | Atira com a arma selecionada no momento |
| `MOUSE2` | Atira com a Shaft (LG / Thunderbolt) enquanto segurado e volta para a arma anterior ao soltar |
| `MOUSE3` | Seleciona a SNG (Super Nailgun) |
| `MOUSE4` | Seleciona a GL (Grenade Launcher) |
| `MOUSE5` | Rocket jump (seleciona a RL, pula e atira) |
| `E` | Seleciona a RL (Rocket Launcher) |
| `R` | Seleciona a GL (Grenade Launcher) |
| `Q` | Seleciona a LG (Lightning Gun) |
| `CAPSLOCK` | Seleciona a SNG (Super Nailgun) |
| `TAB` | Mostra o placar |
| `F12` | Tira um print da tela |

## Comandos

Digite no console (tecla `` ` ``):

| Comando | Descrição |
|---|---|
| `ktx` | Ativa o mod KTX (para jogar com bots) |
| `qwbrktx` | Entra no servidor #1 de KTX do QW Brazil |
| `qwbrktx2` | Entra no servidor #2 de KTX do QW Brazil (dedicado para treino) |
| `qwbrtd2` | Entra no servidor de Total Destruction do QW Brazil |

> O KTX fica em uma pasta separada e **não é carregado automaticamente**, já que a maioria das pessoas joga em servidores. Se quiser jogar com bots, digite `ktx` no console **antes de carregar um mapa ou entrar em um servidor**. Com um mapa já carregado, o comando não consegue trocar para o mod.

## Autor

Pacote montado por **CrazyKillerBR**.

Dúvidas, sugestões ou problemas: chama no Discord **`crazykillerbr`**.

## Créditos

- **[Tiba](https://github.com/tibazera)**: pacote original com a textura cinza e as configurações de otimização para o competitivo.
- **[nQuake](https://nquake.com)** ([GitHub](https://github.com/nQuake)): pacote de texturas usado no competitivo e base das skins deste pacote.
- **[ezQuake](https://github.com/QW-Group/ezquake-source)**: cliente QuakeWorld.
- **[KTX](https://github.com/QW-Group/ktx)**: mod de servidor (Kombat Teams eXtreme).
