# Documentation

Repositório destinado a criação de wikis dos projetos MadDev.

## Tutorial de como contribuir

### 1. Clone o repositório
```bash
git clone git@github.com:MadDevInc/documentation.git
```

### 2. Instalando o mkdocs
Instale o mkdocs atráves do seguinte comando:
```bash
pip install mkdocs
```

### 3. Realize as alterações necessárias

Dentro do diretório `docs` você pode pode encontrar a pasta específica para cada projeto. E em cada projeto, basta alterar o index.html com as informações necessárias.

### 4. Visualizando as alterações

Para rodar o servidor local e checar suas modificações, basta rodar o seguinte comando:
```bash
mkdocs serve
```

### 5. Realize o commit e push
Após garantir a corretude de suas modificações, basta realizar o commit e push para o repositório na branch `main`.

### 6. Deploy do Pages
Para realizar o deploy atráves do mkdocs, basta rodar os seguintes comandos:
```bash
mkdocs build
mkdocs gh-deploy
```

