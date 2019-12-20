# Lab.Primeira-I-D
Laboratório de Redes, edição de  Internet Drafts (I-D)

Exercício de escrita de I-D

Utilize o arquivo draft-HTTP-GPOS-NomeAutor-00.md  para criar sua versão de extensão do protocolo HTTP para permitir a requisição de geolocalização de um *site*. 

Na seção 1, faça uma introdução para que serve seu protocolo. Descreva quais situações esse protocolo é útil. Cite os protocolos que se baseou.

Na seção3, descreva as mensagens do cliente e do servidor:

1. Uma requisição GET HTTP deve incluir um campo **GPOS: nome_dispositivo** 

2. O servidor deve retornar uma resposta no formato:

nome_dispositivo ttl class **GPOS**  longitude latitude altitude

Defina como fazer a extensão para o **PUT**
             
Observações: 

* Os campos  nome_dispositivo, ttl e classe são opcionais na RFC 1712. 
           
* Sua I-D deve ser renomeada de forma que o arquivo inclua seu próprio nome:  draft-HTTP-GPOS-SEU_NOME-00.txt

* Para formatar texto no formato MarkDown verifique o [link](https://github.com/luong-komorebi/Markdown-Tutorial/blob/master/README_pt-BR.md)
