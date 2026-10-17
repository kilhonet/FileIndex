# FileIndex

**Pesquisador de arquivos gratuito para Windows que encontra arquivos em todo o PC assim que você digita um nome.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · Português (Brasil) · [Français](README.fr.md)

> Este documento é uma tradução. Em caso de divergência, a [versão em coreano](README.ko.md) prevalece.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/fileindex?lang=pt)

![Tela do FileIndex](images/fileindex-en.png)

## Visão geral

O FileIndex pesquisa por nome de arquivo em todas as unidades do PC de uma só vez. Os resultados mudam enquanto você digita na caixa de pesquisa, e nomes em coreano podem ser encontrados digitando apenas as consoantes iniciais (`ㅅㅈ` → 설정).

Na primeira execução ele monta uma lista dos arquivos de cada unidade; daí em diante acompanha em tempo real os arquivos criados, excluídos e renomeados, para que os resultados estejam sempre atualizados. Você pode combinar condições de extensão, tamanho, curingas e expressões regulares, e ele também encontra arquivos duplicados com o mesmo nome, tamanho ou conteúdo.

Os arquivos encontrados podem ser abertos, copiados, arrastados e usados com o menu de contexto, como no Explorador de Arquivos. Ao fechar a janela, o FileIndex fica na bandeja do sistema, pronto para voltar na hora, e enquanto está oculto quase não usa memória.

## Recursos

- **Pesquisa enquanto você digita** — encontra nomes que contêm todas as palavras separadas por espaço. Não diferencia maiúsculas de minúsculas.
- **Pesquisa por consoantes iniciais coreanas** — basta digitar `ㅅㅈ` para encontrar nomes como "설정" e "사진".
- **Condições de pesquisa** — extensão (`ext:`), tamanho (`size:`), curingas (`*` `?`), expressões regulares (`regex:`).
- **Localizador de duplicados** — mesmo nome (`dupe:name`), mesmo tamanho (`dupe:size`), conteúdo idêntico (`dupe:content`).
- **Atualização em tempo real** — as mudanças nos arquivos aparecem logo nos resultados. O que mudou enquanto o FileIndex estava fechado é atualizado ao iniciá-lo.
- **Indexação automática de unidades USB** — unidades recém-conectadas são indexadas sozinhas e saem dos resultados quando removidas.
- **Funciona como o Explorador** — clique duplo para abrir, abrir o local, seleção múltipla e cópia, arrastar para o Explorador, menu de contexto do Explorador.
- **Visualização** — mostra ao lado da lista a miniatura do arquivo selecionado (fotos, vídeos, PDFs, documentos do Office e mais).
- **Classificação e destaque** — classifica por nome, caminho, tamanho ou data de modificação; a parte do nome que corresponde é destacada.
- **Fica na bandeja** — ao fechar a janela, ele se esconde na bandeja, onde quase não usa memória.
- **Fica no seu PC** — a lista de arquivos é salva apenas no seu próprio PC.
- **22 idiomas, temas claro e escuro** — segue as configurações do Windows por padrão, ou você mesmo escolhe.

## Download / instalação

| Tipo | Link |
|---|---|
| Instalador | [Baixar](https://down.kilho.net/fileindex?lang=pt) |
| Portátil (ZIP) | [Baixar](https://down.kilho.net/fileindex?lang=pt&nosetup) |

O instalador abre o FileIndex ao terminar e ativa **Executar ao iniciar**, para que ele comece na bandeja sempre que você entrar no Windows. Na versão portátil, descompacte o ZIP e execute `FileIndex.exe`. As duas versões têm os mesmos recursos.

Ler unidades inteiras rapidamente exige direitos de administrador, então o Windows mostra uma janela de confirmação de administrador quando o FileIndex inicia. Clique em **Sim**.

## Uso

### Primeiros passos

1. Execute o FileIndex. Na primeira vez, enquanto ele monta a lista de arquivos de cada unidade, o centro da janela mostra o progresso, por exemplo **C: indexando 42%**. Ao terminar, aparece a tela de pesquisa.
2. Digite parte de um nome de arquivo na caixa de pesquisa. Os resultados aparecem na lista enquanto você digita, e embaixo aparece quantos foram encontrados.
3. Dê um **clique duplo** no arquivo desejado, ou selecione-o com as setas e pressione **Enter**, para abri-lo no programa associado. Pressione **Ctrl+Enter** para abrir a pasta que o contém.
4. Quando terminar, clique no botão de fechar (X) ou pressione **Esc**. O FileIndex não é encerrado: ele se esconde na bandeja. Clique no ícone da bandeja para trazê-lo de volta na hora.

A partir da segunda execução, o FileIndex reaproveita a lista já montada e só atualiza o que mudou enquanto estava fechado, então você pode pesquisar imediatamente.

### Elementos da tela

| Elemento | O que faz |
|---|---|
| Caixa de pesquisa | Digite um nome de arquivo, consoantes iniciais ou condições de pesquisa. O botão de seta à direita pesquisa de novo com o texto atual |
| Lista de resultados | **Nome** · **Caminho** · **Tamanho** · **Data de modificação**. Clique no cabeçalho de uma coluna para classificar; arraste uma borda para mudar a largura |
| Visualização | No canto inferior direito da lista. Miniatura do arquivo selecionado (oculta em arquivos sem miniatura) |
| Barra de status | Número de resultados. Se houver mais que o máximo de resultados, mostra exibidos / total, p. ex. `200 / 14,092 itens` |
| Botão de configurações | Na barra de título, à esquerda do botão de minimizar. Abre a janela **Configurações** |
| Ícone da bandeja | Clique esquerdo para abrir a janela. O menu de contexto tem **FileIndex** · **Autor** · **Sair** |

### Situações de uso

**Encontrar nomes coreanos pelas consoantes iniciais**
Digitando apenas consoantes coreanas, você encontra nomes cujas iniciais aparecem nessa ordem. `ㄱㅇㅅ` encontra nomes como "계약서" e "계약서_수정본", cujas iniciais contêm ㄱ, ㅇ, ㅅ em sequência. Até nomes longos são encontrados com poucas teclas.

**Refinar com várias palavras**
Separe as palavras com espaços e só ficam os nomes que contêm todas elas. `relatorio 2026` encontra arquivos com "relatorio" e "2026" no nome. A ordem das palavras não importa.

**Encontrar só certos tipos de arquivo**
Escreva as extensões depois de `ext:`, separadas por **ponto e vírgula (;)**. As pastas ficam de fora; só aparecem arquivos.
- `ext:pdf` — todos os arquivos PDF
- `ext:jpg;png;gif viagem` — imagens com "viagem" no nome

**Encontrar arquivos grandes para liberar espaço**
Use `size:` para uma condição de tamanho. As unidades são `b` `kb` `mb` `gb` `tb`; sem unidade, são bytes.
- `size:>1gb` — arquivos maiores que 1 GB
- `size:1mb-5mb` — de 1 MB a 5 MB, inclusive (`1mb..5mb` também funciona)
- `ext:mp4 size:>500mb` — vídeos acima de 500 MB

Classifique os resultados pelo cabeçalho **Tamanho** para ver primeiro os maiores arquivos.

**Definir o formato de um nome com curingas**
`*` corresponde a qualquer quantidade de caracteres e `?` a exatamente um. Com curingas, **o nome inteiro** precisa corresponder ao padrão.
- `*.txt` — arquivos com extensão txt
- `readme*` — nomes que começam com readme
- `IMG_????.jpg` — imagens com quatro caracteres depois de IMG_

**Pesquisar com mais precisão usando expressões regulares**
Escreva uma expressão regular depois de `regex:`. Não diferencia maiúsculas de minúsculas e pode corresponder em qualquer parte do nome. Use `^` e `$` para fixar o início e o fim; como os espaços separam os termos de pesquisa, escreva um espaço dentro do padrão como `\s`.
- `regex:^\d{8}` — nomes que começam com oito dígitos (como uma data)
- `regex:(draft|final)` — nomes que contêm draft ou final

Se uma condição estiver escrita errado, a barra de status mostra um exemplo da forma correta.

**Limpar arquivos duplicados**
`dupe:` agrupa os arquivos correspondentes e os mostra grupo por grupo. Combinado com outras condições, compara apenas dentro desses resultados.
- `dupe:name` — arquivos com o mesmo nome (sem diferenciar maiúsculas)
- `dupe:size ext:jpg` — imagens do mesmo tamanho
- `dupe:content ext:mp4` — vídeos com **exatamente o mesmo conteúdo**

O `dupe:content` lê os arquivos de verdade para compará-los, então a barra de status mostra o progresso como **Comparando conteúdo — arquivos n/N, x/y MB**. Mudar o texto da pesquisa interrompe a comparação. Em cada grupo, selecione tudo exceto a cópia que quer manter e depois clique direito → Excluir.

**Encontrar um arquivo recém-baixado**
A classificação padrão é **Data de modificação**, do mais recente para o mais antigo, então basta digitar parte de um nome para o arquivo baixado ou editado mais recentemente ficar no topo. Arquivos novos ou recém-salvos aparecem logo nos resultados.

**Resultados demais / quer ver todos**
Por padrão a lista mostra até **200** resultados. A pesquisa sempre abrange tudo, classifica e mostra a partir do topo — então você vê "os 200 mais recentes" ou "os 200 maiores". `200 / 14,092 itens` na barra de status significa que 200 de 14.092 resultados estão sendo exibidos. Para ver mais, aumente **Configurações → Máx. de resultados**.

**Copiar ou mover vários arquivos para outro lugar**
- Selecione vários com **Ctrl/Shift + clique** ou **Shift + setas**, ou pressione **Ctrl+A** para selecionar todos os resultados.
- Pressione **Ctrl+C** e cole no Explorador de Arquivos.
- Você também pode **arrastar os arquivos selecionados para o Explorador ou para a área de trabalho**. Como no Explorador, eles são movidos na mesma unidade e copiados para outra unidade.

**Usar o menu de contexto do Explorador**
Clique com o botão direito em um resultado para ver o mesmo menu do Explorador (Abrir com, Enviar para, compactar, Excluir, Propriedades etc.). Segure **Shift** ao clicar com o botão direito para ver também os comandos estendidos. Os programas iniciados por esse menu rodam com direitos normais de usuário, não como administrador.

**Ver fotos e documentos sem abri-los**
Com a **Visualização** ligada (padrão), a cada arquivo selecionado aparece uma miniatura no canto inferior direito da lista. É a mesma miniatura do Explorador, então vídeos, PDFs e documentos do Office também são visualizados, além de fotos. Percorra-os com as setas.

**Pesquisar em pendrives e discos externos**
Conecte um e em poucos segundos ele é indexado e entra nos resultados. Ao desconectá-lo, seus resultados somem; ao reconectar, ele é indexado de novo.

**Só com o teclado**
O foco fica sempre na caixa de pesquisa, então é só digitar.

| Tecla | Ação |
|---|---|
| ↑ ↓ / PgUp PgDn | Selecionar resultados (segure Shift para selecionar um intervalo) |
| Enter | Abrir no programa associado (o primeiro resultado se nada estiver selecionado) |
| Ctrl+Enter | Abrir o local do arquivo no Explorador |
| Ctrl+A / Ctrl+C | Selecionar todos os resultados / copiar os arquivos selecionados |
| Esc | Limpar o texto da pesquisa; se já estiver vazio, esconder na bandeja |

**Abrir uma pesquisa direto de um atalho ou script**
Passe uma pesquisa depois de `--search` (ou `-s`) e o FileIndex abre com esses resultados. Se o FileIndex já estiver rodando, a janela aberta faz essa pesquisa.

```
FileIndex.exe --search "ext:pdf contrato"
FileIndex.exe -s "*.psd"
```

Coloque isso no destino de um atalho da área de trabalho para abrir uma pesquisa frequente com um clique.

**Deixar rodando e usar como um atalho de teclado**
Com **Executar ao iniciar** ligado, o FileIndex começa na bandeja, sem janela, quando você entra no Windows. Clique no ícone da bandeja quando precisar — ele aparece com o cursor já na caixa de pesquisa, então é só digitar. Para encerrar de vez, clique direito no ícone da bandeja → **Sair**.

## Configuração

Abra **Configurações** pelo botão de configurações na barra de título. As mudanças são salvas e aplicadas na hora.

| Seção | Item | Padrão |
|---|---|---|
| Geral | Classificação padrão (Por nome · Por caminho · Por tamanho · Por data de modificação) | Por data de modificação |
| Geral | Tema (Sistema · Claro · Escuro) | Sistema |
| Geral | Idioma (Sistema + 22 idiomas) | Sistema |
| Geral | Máx. de resultados | 200 |
| Geral | Visualização | Ligada |
| Geral | Executar ao iniciar | Ligado na versão com instalador |
| Sobre | Versão · Autor · Página inicial · Licença | — |

**[Redefinir]** restaura as configurações padrão e também desliga Executar ao iniciar. A lista de arquivos já montada é mantida. Ao mudar o idioma, a tela passa para esse idioma na hora, sem reiniciar.

## Requisitos

- Windows 10 · Windows 11 (64 bits)
- Unidades formatadas em NTFS (o formato padrão do Windows — tanto discos internos quanto unidades USB)
- Direitos de administrador (clique em **Sim** na confirmação ao iniciar)
- A internet é usada só para verificar novas versões. A pesquisa funciona offline.

## Atualizações

O FileIndex **não** se atualiza sozinho. Ao iniciar, ele verifica se há uma nova versão e mostra um aviso; clicar em **[Sim]** abre a página de download e fecha o programa. As novas versões são publicadas manualmente após testes internos e anunciadas na [página do FileIndex](https://kilho.net/fileindex). Veja o [aviso sobre a política de atualização](https://en.kilho.net/archives/notice/2940).

## Licença

O FileIndex é **freeware**. Use-o gratuitamente em qualquer lugar — no escritório, em casa, em órgãos públicos ou na escola — e redistribua-o livremente.

## Links

- Site: <https://kilho.net/fileindex>
- Fórum: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
