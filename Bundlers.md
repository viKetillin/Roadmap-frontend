# O que são Bundlers no React

Em resumo, um **bundler** é uma ferramenta que agrupa todo o projeto React em um único arquivo, ou em poucos arquivos, que serão executados no navegador. Ele é utilizado para melhorar a performance da aplicação, reduzir o tamanho do código e diminuir o número de requisições HTTP realizadas pelo navegador para carregar o conteúdo.

Os bundlers também possuem ferramentas integradas que auxiliam na **transpilação de JSX e JavaScript moderno para JavaScript compatível com o navegador**, além de manipular arquivos de estilo, transformando-os em CSS compreensível pelo browser.

---

## Como funcionam os bundlers

### 1. Criação do grafo de dependências

Primeiramente, o bundler percorre todos os arquivos importados, começando pelo **entry point**, criando uma estrutura semelhante a um grafo. Ele inicia a leitura pelo arquivo `index.js` (ou outro ponto de entrada configurado) e mapeia todas as dependências vinculadas a ele.

---

### 2. Resolução de módulos

Após a criação do grafo de dependências, o bundler identifica quais dependências são bibliotecas provenientes dos módulos do Node.js e quais são arquivos locais do projeto.

---

### 3. Transpilação (nem sempre obrigatória)

Quando determinados elementos não podem ser executados diretamente no navegador — como **TypeScript** ou **JSX** — os bundlers utilizam transpiladores, como o **Babel**, para transformar esse código em JavaScript compreensível pelo navegador.

---

### 4. Tree Shaking

Nesta etapa, o bundler otimiza o bundle final removendo código desnecessário, como importações não utilizadas.

**Obs.:** Para aproveitar o máximo do *tree shaking*, é essencial:

- Utilizar **ES Modules**
- Evitar efeitos colaterais nos módulos (como manipulação direta do DOM)
- Garantir que o `package.json` contenha a propriedade `"sideEffects": false`

---

### 5. Minificação e compressão

Os arquivos finais são compactados para serem enviados mais rapidamente pela rede. Isso inclui a remoção de espaços em branco, comentários e a redução de nomes de variáveis, tornando o código menor e mais eficiente.

---

### 6. Code Splitting

Essa funcionalidade, presente nos bundlers modernos, permite dividir a aplicação em múltiplos bundles. Isso melhora significativamente o tempo de carregamento, especialmente em projetos grandes.

Uma abordagem comum é gerar um bundle por rota da aplicação e utilizar **lazy loading**, carregando apenas o código necessário conforme o usuário navega.

---

### 7. Geração da saída

Após todo o processamento — transpilação, otimização e divisão de código — o bundler gera os arquivos finais, que são salvos no diretório de saída definido na configuração do projeto.

---

## Bundlers mais populares no React

### Webpack

O **Webpack** é um dos bundlers mais populares no ecossistema React. Ele oferece um processo de build altamente configurável e extensível, sendo amplamente adotado pela comunidade.

---

### Parcel

O **Parcel** é conhecido por sua facilidade de uso e abordagem *zero configuration*. É uma excelente escolha para projetos menores ou para desenvolvedores que preferem simplicidade.

---

### Rollup

O **Rollup** é um bundler especializado, utilizado principalmente para bibliotecas e pacotes. Destaca-se por suas excelentes capacidades de *tree shaking*, gerando bundles altamente otimizados.

---

## Conclusão

Os bundlers desempenham um papel crucial no desenvolvimento web moderno, especialmente em aplicações React. Eles otimizam o processo de preparação do código para o navegador ao agrupar múltiplos arquivos, reduzir o tamanho final do bundle e melhorar o desempenho da aplicação.

Por meio da criação de um grafo de dependências, resolução de módulos, transpilação e otimizações como *tree shaking*, minificação e divisão de código, os bundlers garantem que o resultado final seja eficiente e pronto para produção. Compreender seu funcionamento contribui diretamente para um melhor fluxo de desenvolvimento e aplicações mais performáticas.

---

## Fontes

- https://medium.com/@krishnakeshri_30423/the-crucial-role-of-bundlers-in-react-development-bca6c67c1681
- https://benizcode.hashnode.dev/what-is-a-bundler
- https://medium.com/@ashwilder/what-is-a-bundler-and-how-to-use-it-in-react-development-ec5f2c562a11
