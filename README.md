# estudo-less

## COMANDOS

compilar: lessc estilos.less estilos.css

instalar grunt: npm install -g grunt

instalar cli do grunt: sudo npm install -g grunt-cli

instalar plugins do grunt: sudo npm install grunt grunt-contrib-less grunt-contrib-watch jit-grunt --save-dev

rodar grunt: grunt

### Mixins e extends  
A sintaxe para definir um mixin é o mesmo de uma classe css .sombra-padrao($padrao:10px){box-shadow: 0px 0px $padrao black;}.  
Para criar um extend posso usar um mixin que já foi criado, para chamar esse mixin criando um extend basta colocar no arquivo less assim: &:extend(.sombra-padrao).  
#### Diferença  
A diferença entre um mixin e o extend é que o mixin você pode passar um valor para ele na hora de adicionar já o extend não, mas o extend ele junta todos os elementos css que estão utilizando o extend no css ficaria algo mais ou menos assim: buton, p, h1{todo o css}. O extend já junta todo mundo automaticamente.  


### Isolar media query em variaveis  
A sintaxe seria essa: @mobile: ~"(max-width: 980px)";, porque estou passando uma string para uma variável, então além das "" devo coloca o sinal de ~ no início do media query.  

#### Fazendo calculos no less  
para fazer calculos no less é bem simples é só fazer uma operação matemática comum 16 * 3px.