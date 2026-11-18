# ATLAS — Ouse ir! | MVP 2027

Projeto inicial criado do zero com **HTML5 e CSS3**, sem JavaScript e sem banco de dados.

## Países incluídos nesta versão
- Brasil
- Estados Unidos
- Israel

Os outros países não foram criados nesta entrega. A estrutura está preparada para você adicioná-los manualmente.

## 1. Como salvar no seu computador (Debian / Linux)

1. Baixe o arquivo `ATLAS_2027.zip`.
2. Abra a pasta **Downloads**.
3. Clique com o botão direito no ZIP e escolha **Extrair aqui**.
4. Mova a pasta extraída `ATLAS_2027` para seu diretório de projetos. Sugestão:

   `~/Desenvolvimento/02-PROJETOS/atlas/`

5. Se já existir uma pasta `atlas`, não substitua tudo sem conferir. Você pode renomear a pasta extraída para `atlas-mvp-2027` e comparar os arquivos primeiro.
6. Abra a pasta no VS Code: **Arquivo → Abrir Pasta**.
7. Abra `index.html` no navegador para visualizar o site.

## 2. Abrir pelo terminal

Depois de extrair o ZIP, você pode executar:

```bash
cd ~/Desenvolvimento/02-PROJETOS/atlas/ATLAS_2027
code .
```

Se `code .` não funcionar, abra o VS Code pelo menu e use **Arquivo → Abrir Pasta**.

Para abrir a página inicial no navegador a partir do terminal:

```bash
xdg-open index.html
```

## 3. Estrutura de pastas

```text
ATLAS_2027/
├── index.html
├── README.md
├── css/
│   └── estilo.css
├── paises/
│   ├── brasil.html
│   ├── estados-unidos.html
│   └── israel.html
├── modelos/
│   └── modelo-pais.html
├── conteudo/
│   ├── colecoes/
│   ├── gastronomia/
│   ├── cultura/
│   ├── ciencia-tecnologia/
│   ├── esportes/
│   ├── historia/
│   └── natureza/
├── documentos/
│   ├── planejamento/
│   └── referencias/
├── imagens/
│   ├── bandeiras/
│   ├── paises/
│   ├── cidades/
│   ├── atracoes/
│   └── icones/
├── missoes/
├── colecoes/
└── emblemas/
```

## 4. Como criar um quarto país

1. Abra `modelos/modelo-pais.html`.
2. Copie o arquivo.
3. Salve a cópia dentro de `paises/`, usando um nome simples, por exemplo `japao.html`.
4. Substitua os textos de exemplo pelo conteúdo do novo país.
5. Ajuste o título da página, nome, bandeira, região, resumo e seções.
6. Na `index.html`, copie um dos cartões de país e altere o nome, resumo, bandeira e link para `paises/japao.html`.

**Atenção aos caminhos:** páginas dentro de `paises/` usam `../css/estilo.css` para acessar o CSS e `../index.html` para voltar à página inicial. A página inicial usa `css/estilo.css`.

## 5. Como adicionar imagens

Coloque cada imagem na pasta correspondente dentro de `imagens/`. Exemplo:

- Bandeiras: `imagens/bandeiras/`
- Países: `imagens/paises/`
- Cidades: `imagens/cidades/`
- Atrações: `imagens/atracoes/`

Em páginas dentro de `paises/`, o caminho começa com `../imagens/...`.

Exemplo:

```html
<img src="../imagens/paises/brasil-amazonia.jpg" alt="Paisagem da Floresta Amazônica">
```

Use imagens próprias, de domínio público ou com licença que permita o uso. Guarde a fonte e a licença em `documentos/referencias/`.

## 6. O que funciona agora

- Navegação entre a página inicial e os três países.
- Links internos para as seções.
- Layout responsivo para computador, tablet e celular.
- Conteúdo estático disponível sem servidor e sem banco de dados.
- Modelo HTML para criar novas páginas de países.

## 7. O que ainda não funciona (fica para etapas futuras)

- Login e perfil real.
- Salvamento automático do Diário de Bordo.
- XP, níveis e dólares virtuais calculados automaticamente.
- Checklists marcáveis com persistência.
- Busca e filtros dinâmicos.
- Mapas interativos e geolocalização.
- Banco de dados, sincronização e painel administrativo.

Esses recursos exigem JavaScript e/ou backend. Não estão simulados como se fossem funções reais.

## 8. Boas práticas

- Use nomes de arquivos em minúsculas, sem espaços e sem acentos.
- Mantenha um único arquivo CSS compartilhado para o visual geral.
- Ao adicionar conteúdo, registre as fontes e a data de consulta.
- Para vistos, leis, fusos, eventos, segurança e indicadores, confirme informações atualizadas em fontes oficiais.
- Faça cópias de segurança antes de grandes alterações.

## 9. Primeiro passo recomendado

Abra `index.html`, explore os três países e depois escolha um deles para revisar o conteúdo. Só depois comece a criar os demais países a partir do modelo.
