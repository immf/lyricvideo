# lyricvideo

Gerador de lyric videos estilizados para Windows: um único `lyricvideo.exe` (cerca de 0,7 MB, sem instalação e sem dependências). Ele busca a letra sincronizada no LRCLIB, analisa a música (energia, ataques, BPM) e anima a letra no ritmo com 16 estilos (neon, metal, punk, gótico, heavy demoníaco, papel, karaokê, Natal, Halloween e outros). Exporta MP4, ou MOV/WebM/PNG com fundo transparente.

## Como usar

1. Baixe o repositório (Code > Download ZIP) e extraia.
2. Rode `lyricvideo.exe` e arraste uma música ou um clipe para a janela. Artista e título saem do nome do arquivo, e a letra é buscada sozinha.
3. Escolha o estilo, veja o preview e clique em Exportar. Os vídeos vão para `output\`.

Requer Windows 10 ou superior. O `ffmpeg.exe` é opcional: só é usado para formatos que o Windows não abre e para exportar com transparência (coloque-o ao lado do exe ou no PATH).

## Conteúdo

| Pasta / arquivo | O que é |
| --- | --- |
| `lyricvideo.exe` | o aplicativo (interface gráfica, ou linha de comando com `--help`) |
| `docs/manual.htm` | manual completo: estilos, edição da letra, fundo, exportação, linha de comando |
| `docs/arquitetura.htm` | como o vídeo é gerado: pipeline, Direct2D, análise de áudio, codificação |
| `estilos/` | presets de estilo editáveis (`.ini`); modelos comentados em `estilos/_modelos/` |
| `fonts/` | 29 fontes livres (licenças OFL e Apache 2.0, com o texto da licença em cada pasta) |

Os `.htm` são arquivos únicos (imagens embutidas): abra-os no navegador depois de baixar.
