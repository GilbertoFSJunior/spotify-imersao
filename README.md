# Spotify Clone - Imersão Alura

Este projeto é uma interface de usuário inspirada no Spotify, desenvolvida durante a Imersão Alura. Ele simula funcionalidades básicas de um player de música, incluindo busca por artistas, exibição de playlists e interação com elementos visuais.

## Estrutura do Projeto

A estrutura do projeto é organizada da seguinte forma:

```
.
├── artists.json
├── index.html
├── README.md
├── script.js
├── search.js
├── SpotifyImage.png
├── SpotifyImage1.png
├── api-artists/
│   └── artists.json
├── src/
│   ├── assets/
│   │   ├── icons/
│   │   │   ├── favicon.png
│   │   │   ├── logo-spotify.png
│   │   │   ├── search.png
│   │   │   ├── small-left.png
│   │   │   └── small-right.png
│   │   └── playlist/
│   │       ├── 1.jpeg
│   │       ├── 2.png
│   │       ├── ...
│   ├── styles/
│       ├── main-content.css
│       ├── main-content-rem.css
│       ├── media-query.css
│       ├── reset.css
│       ├── sidebar-footer.css
│       ├── sidebar-footer-rem.css
│       └── vars.css
```

## Funcionalidades

### 1. **Busca por Artistas**
- O arquivo `search.js` implementa a funcionalidade de busca por artistas. Ele utiliza a API local (`api-artists/artists.json`) para buscar artistas com base no termo digitado no campo de busca.

### 2. **Exibição de Playlists**
- As playlists são exibidas como cartões na página principal. Cada cartão possui uma imagem e um título, representando diferentes categorias de música.

### 3. **Saudação Dinâmica**
- O arquivo `script.js` exibe uma saudação dinâmica ("Bom dia", "Boa tarde" ou "Boa noite") com base no horário atual.

### 4. **Design Responsivo**
- O projeto utiliza CSS responsivo para se adaptar a diferentes tamanhos de tela. Arquivos como `media-query.css` e `vars.css` ajudam a ajustar o layout para dispositivos móveis e desktops.

## Tecnologias Utilizadas

- **HTML5**: Estrutura da página.
- **CSS3**: Estilização e responsividade.
- **JavaScript**: Interatividade e manipulação do DOM.
- **JSON**: Simulação de uma API para dados de artistas.
- **Font Awesome**: Ícones para navegação e interação.

## Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/spotify-clone.git
   cd spotify-clone
   ```

2. Instale o [JSON Server](https://github.com/typicode/json-server) para simular a API:
   ```bash
   npm install -g json-server
   ```

3. Inicie o servidor JSON:
   ```bash
   json-server --watch api-artists/artists.json --port 3000
   ```

4. Abra o arquivo `index.html` em seu navegador.

## Estrutura de Dados

### `api-artists/artists.json`
Este arquivo contém informações sobre os artistas, incluindo:
- `id`: Identificador único.
- `name`: Nome do artista.
- `genre`: Gênero musical.
- `urlImg`: URL da imagem do artista.

Exemplo:
```json
{
  "artists": [
    {
      "id": 1,
      "name": "Foo Fighters",
      "genre": "Rock",
      "urlImg": "https://i.scdn.co/image/ab67616100005174c884df599abc793c116cdf15"
    }
  ]
}
```

## Estilização

Os estilos estão organizados em múltiplos arquivos CSS:
- **`reset.css`**: Remove estilos padrão dos navegadores.
- **`vars.css`**: Define variáveis globais para cores, fontes e espaçamentos.
- **`main-content.css`**: Estiliza o conteúdo principal.
- **`sidebar-footer.css`**: Estiliza a barra lateral e o rodapé.
- **`media-query.css`**: Adapta o layout para diferentes tamanhos de tela.

## Melhorias Futuras

- Implementar um player funcional para reproduzir músicas.
- Adicionar autenticação de usuário.
- Conectar a uma API real, como a do Spotify.
- Melhorar a responsividade para dispositivos menores.

## Créditos

Este projeto foi desenvolvido durante a **Imersão Alura**, com o objetivo de praticar habilidades de front-end e simular a interface de um aplicativo popular.

## Licença

Este projeto é de uso educacional e não possui fins comerciais. Todos os direitos sobre a marca e design do Spotify pertencem aos seus respectivos proprietários.
```
