**Working Group Name**  **Initial. Lastname**
  
Internet Draft         DComp/UFS

Intended status: EXPERIMENTAL         XXX 0, 0000

Expires: Fail 0000



# Title draft-GRUPO-DE-TRABALHO-NOME-ALUNO-00.txt


## Status of this Memo

This Internet-Draft is submitted in full conformance with the provisions of BCP 78 and BCP 79. 
This document may not be modified, and derivative works of it may not be created, except to publish
it as an RFC and to translate it into languages other than English.

This document may contain material from IETF Documents or IETF Contributions published or made publicly 
available before November 10, 2008. The person(s) controlling the copyright in some of this material may 
not have granted the IETF Trust the right to allow modifications of such material outside the IETF Standards Process. 
Without obtaining an adequate license from the person(s) controlling the copyright in such materials, this document may
not be modified outside the IETF Standards Process, and derivative works of it may not be created outside the IETF
Standards Process, except to format it for publication as an RFC or to translate it into languages other than English.

Internet-Drafts are working documents of the Internet Engineering Task Force (IETF), its areas, and its working groups. 
Note that other groups may also distribute working documents as Internet-Drafts.
Internet-Drafts are draft documents valid for a maximum of six months and may be updated, replaced,
or obsoleted by other documents at any time.  It is inappropriate to use Internet-Drafts as reference material or to cite
them other than as "work in progress."
The list of current Internet-Drafts can be accessed at http://www.ietf.org/ietf/1id-abstracts.txt
The list of Internet-Draft Shadow Directories can be accessed at http://www.ietf.org/shadow.html
This Internet-Draft will expire on Fail 19, 0000.

## Copyright Notice
Copyright (c) 0000 IETF Trust and the persons identified as the document authors. All rights reserved.

This document is subject to BCP 78 and the IETF Trust’s Legal Provisions Relating to IETF Documents 
(http://trustee.ietf.org/license-info) in effect on the date of publication of this document. Please
review these documents carefully, as they describe your rights and restrictions with respect to this document. 	

## Abstract
> Type your abstract here. Typically 5-10 lines, never less than 3 lines nor more than 20 lines 


## 1. Introduction
 Tendo em vista a necessídade de melhor precisão na hora da localização de usuários e definição de rotas desejadas por aplicativos como o google maps, faz-se necessário um protocolo HHTP que dispinibilize a localização e transferencia de informações baseadas em geolocalização.
 O GPOS é um Protocolo que possibilita a geolocalização.

## 2. Conventions used in this document
In examples, "C:" and "S:" indicate lines sent by the client and server respectively.
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 [RFC2119]. 

In this document, these words will appear with that interpretation   only when in ALL CAPS. Lower case uses of these words are not to be    interpreted as carrying significance described in RFC 2119.

In this document, the characters ">>" preceding an indented line(s)   indicates a statement using the key words listed above. This convention aids reviewers in quickly identifying or finding the portions of this RFC covered by these keywords.

## 3. Descrição do Protocolo
Uma mensagem HTTP com um camo GPOS que ao ser enviada pelo cliente teremos O nome do dispositivo que está enviando a mensagem e o destino.

MKensagem Cliente:
GET / HTTP/1.1
Host: developer.mozilla.org
GPOS: nome_dispositivo, Destino

Quando respondida pelo servidor o campo GPOS envia informações meridionais e uma rota considerando as informações meriodionais.

Mensagem Servidor:
 HTTP/1.1 200 OK
 Date: Sat, 09 Oct 2010 14:28:02 GMT
 Server: Apache
 Last-Modified: Tue, 01 Dec 2009 20:18:22 GMT
 ETag: "51142bc1-7449-479b075b2891b"
 Accept-Ranges: bytes
 Content-Length: 29769
 Content-Type: text/html 
 GPOS: Longitude, Latitude, Graus, Rotas
 
 
SENDO:
  LONGITUDE:Descrição da localização de um lugar na Terra medido em graus, de zero a 180 para leste ou para oeste, a partir do                              Meridiano de Greenwich.
  Latitude:È a coordenada geográfica ou geodésica definida na esfera, no elipsoide de referência ou na superfície terrestre, que   é o ângulo entre o plano do equador e a normal à superfície de referência.
  Graus: angulação geral da rota do dispisitivo
  Rotas: a rota mais apropriada gerada pela aplicação considerando aspectos importantes como locais perigosos.


## 4. Security Considerations

>Add any security considerations

## 5. IANA Considerations

>Add any IANA considerations

## 6. Conclusions
> Add any conclusions

## 7. References

### 7.1. Normative References

[1]	Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels", BCP 14, RFC 2119, March 1997.

[2]	Crocker, D. and Overell, P.(Editors), "Augmented BNF for Syntax Specifications: ABNF", RFC 2234, Internet Mail Consortium and 
Demon Internet Ltd., November 1997.

[RFC2119]	Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels", BCP 14, RFC 2119, March 1997.

[RFC2234]	Crocker, D. and Overell, P.(Editors), "Augmented BNF for Syntax Specifications: ABNF", RFC 2234, Internet Mail 
Consortium and Demon Internet Ltd., November 1997.

### 7.2. Informative References

[3]	Faber, T., Touch, J. and W. Yue, "The TIME-WAIT state in TCP and Its Effect on Busy Servers", Proc. Infocom 1999 pp. 1573-1583.
[Fab1999]	Faber, T., Touch, J. and W. Yue, "The TIME-WAIT state in TCP and Its Effect on Busy Servers", Proc. Infocom 1999  
pp. 1573-1583.

## 8. Acknowledgments
>Add any acknowledgements
