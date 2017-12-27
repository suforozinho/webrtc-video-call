# webrtc-video-call
Um aplicativo que faz vídeo chamada com aquele que estão na LAN
## Como usar  
Clone ou baixe o repositório, e na pasta raíz execute `npm install`.  
Logo após, ainda na pasta raíz, execute `npm run webpack`.
Depois de fazer essas coisas você está pronto para iniciar um servidor para fazer as vídeos chamadas.  
Para isso execute, na raíz do projeto, esse comando: `http-server`.
depois disso, abra outro terminal(deixe o outro terminal rodando o comando de cima) e execute: `local-ssl-proxy --source 8081 --target 8080`.
No output do `http-server` haverá dois endereços, acesse o que começa com 192, substituindo http por https, e mudando o porte 8080 para 8081. Vai ficar assim por exemplo: https://192.168.1.8:8081/.
Depois de acessar, permita que o browser acesse o site, pois ele vai te dar um alerta de segurança(não tem perigo nenhum ;) ).

Não se esqueça de criar seu próprio arquivo `.env`.
