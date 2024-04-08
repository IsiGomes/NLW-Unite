# HTML - Linguagem de marcação de hipertexto (HypertextMarkutLanguage)
*Hypertext*
Tem haver com uma tag especifica chamada tag link/ tag a (a hybertext link) e href endereço de referencia EX: <a href="http://google.com>google.com</a> gera um link 

*Markup* 
Html sempre tem tags/marcações e tem abertura fechamento < >/ Nem todas as tags tem fechamento mas a maioria sim EX: <h1> texto...<h1/> essa é uma intruçao para o html escrever algo 

*Language* É a sintese que conversamos com a maquina / Visualmente usa estilos que já sao do nosso navegador / EX:

<table width ="100%"> #table para criar tabela #width para tabela adquirir largura
  <thead style="text-align: left"> #Cabeçario #Style ="" para arrumar texto
    <tr>
      <th>Participantes</th>
      <th>Data da Inscrição</th>
      <th>Dada do Check-in</th>
    </tr>
  </thead> #linha da cabeça/cabeçario

  <tbody> #desenvolvendo corpo da tabela
    <tr>
      <td>
        <strong> #para negrito/letra forte
          Diego Fernandes
        </strong> #para negrito/letra forte
        <br> #break / quebra de linha
        <small> #texto com letra pequena
          diego@gmail.com
        </small> #texto com letra pequena
     </td>
      <td> há 3 dias</td>
      <td>há 3 minutos</td>
    </tr>
  </tbody> #desenvolvendo corpo da tabela
</table> #terminar tabela 


# CSS
*Cascading StyleSheet*
```css 
/*declarações*/
body{
  background-color: black;
  color: #ffffff;
}
```

# JavaScript - Sintase e Lógica
// Variaveis = Guardar a informação para usar mais tarde
existe palavras marcadas para instruçao de Variaveis EX: Const mensagem = ... , mais tarde ao usar a mensagem o Java trás pra mim a informação que guardei em mensagem
//serve para que eu possa usar mais de uma vez alguma informação e para que eu possa organizar os meus dados.
//Posso colocar qualquer coisa dentro de uma variavel e uma função é uma dessas coisas

// Tipo de dado = É a informação, pode ser numero/number, texto/string entre outras

// Função é como guardar codigos dentro de um arquivo determinado pelo nome que é dado a função podendo ser usado posteriormente e também podemos dar instruções a função
//a função alert (...) exemplo abre um caixinha onde guardamos qualquer informção como uma pasta do computador
//serve para executar informçães de maneira programavel

EX: //objeto Javascript
const participante = {
  nome: "Mayk Brito",
   email: "MaykBrito@gmail.com",
    DataInscricao: new Date(2024, 2, 22, 19, 20),
     DataCheckin: new Date (2024, 2, 25, 22, 00)    

}
 //Criar variaveis para lista 
 let participantes = [
  {
    nome: "Mayk Brito",
   email: "MaykBrito@gmail.com",
    DataInscricao: new Date(2024, 2, 22, 19, 20),
     DataCheckin: new Date (2024, 2, 25, 22, 00)
  },
 ]

const CriarNovoParcticipante = (participante) => {
 return `
 <tr>
   <td>
      <strong> 
          ${participante.nome}
        </strong>
        <br>
        <small>
         ${participante.email}
      </small>
    </td>
    <td> ${participante.DataInscricao}</td>
  <td> ${participante.DataCheckin}</td>
 </tr>
 `
// => isso se chama função arrow
// document é um objeto JavaScript que é como se fosse um objeto da vida real, se você imaginar um relógio ele tem funcionalidades/ funções, entao objetos tem funções e também tem propriedades, um relógio tem cor, tem peso etc e eu consigo entrar dentro de um objeto e pegar essas funçoes ou propriedades colocando um pontinho
//QuerySelector/Seletor de pesquisas
//for(let participante of participantes) é uma estrutura de repetiçao/loop cria uma variavelde participantes repetidamente até finalizar a lista 
//day.js possui diversos codigos prontos  


certificado # https://app.rocketseat.com.br/certificates/82709446-97bd-4eed-a240-2e99f6c7b610