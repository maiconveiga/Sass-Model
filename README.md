# Sobre SASS

npm list -g --depth=0

Pré processador para css
Recursos
Variáveis

# Estrutura de pastas

src -> dist
build

# Instalação

- Instalar o nodejs versão LTS (Long term support)
- Testar a versão no terminal node
- Instalar o sass mo terminal npm i -g sass  -> instalar de forma global
- Instalar o pacote do VSCode SASS

# Existem basicamente dois tipos de extensões sass
- .sass
- .scss -> mais usada

# Iniciar o npm

- npm init -> Dar enter em todas as opções
- npm i --save-dev sass -> Instalar dentro da dependência do projeto
- dentro de package.json, criar um script "sass": "sass",
- na sequência, executat npm run sass -watch

# Declarar variáveis

- $nomeVariavel

## Pode ser usado uma variável de outro .scss 
- @use 'nomeDoModulo';
- nomeDoModulo.$nomeDaVariavel; 

# Pseudo classe
- &:hover{}

# Criar módulos
- @use 'nomeDoModulo';

# Uso do mixin

- O @mixin deve estar no topo da página
@mixin nomedoMixin(){
    atributos
}

- Aqui irá conter todas as configurações
elemento{
    @include nomeDoMixin();
}
elemento2{
    @include nomeDoMixin();
    outros atributos quaisquer
}

# Uso de operadores

&:hover{background-color: darken(cor, 0,7)}
&:hover{background-color: lighten(cor, 0,7)}