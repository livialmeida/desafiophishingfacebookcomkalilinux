# Desafio Phishing de Clonagem da Página de login do Facebook 

### **Objetivo**
Demonstrar como realizar a clonagem da página de login do Facebook usando  o Kali Linux e o SET (Social-Engineer Toolkit), configurando adequadamente para captura de credenciais em um ambiente controlado.

### **Requisitos**
- Sistema Operacional: Kali Linux
- Navegadores: Google Chrome, Mozilla Firefox, Internet Explorer/Microsoft Edge
- Permissão para testes em ambiente controlado, sem a exposição de terceiros e eventuais violaçôes à LGPD

### **Passo a Passo**
1) Entrar como root no terminal
2) Inicie o SET
3) Escolher a opção 2 do menu (2 - Website Attack Vectors)
4) Dentro desta opção, selecionar o 3º método apontado (3 - Credential Harvester Attack)
5) Após, escolher o método de clonagem de site (Opção 2 - Site Cloner)
6) Inserir a URL completa do Facebook (http://www.facebook.com) para clonar

## **Resultados preliminares**
Observações importantes:
- O primeiro teste não deu certo, foi realizado em guia anônima do navegador Google Chrome conforme ensinado pelo instrutor. Este primeiro teste ocorreu na data de 28/12/2024.
- Outros testes passaram a ser feitos sem alteração no html da página clonada em 31/12/2024. Eles foram realizados novamente no Google Chrome (guia normal e anônima), Microsoft Edge e Mozilla Firefox no sistema operacional Windows 10.
- Também foi realizado teste no navegador Internet Explorer do Windows 7 instalado no VirtualBox conforme abaixo:
![image](https://github.com/user-attachments/assets/c24941ed-4e3f-485e-a863-64fc88c4b872)

## **Não desistirei de tentar clonar a página de login do Facebook e ter êxito no desafio!**

## **Considerações e possíveis justificativas sobre os motivos dos erros de clonagem**
1) Foi observado a existência de problemas técnicos na url indicada. Os navegadores exibiram alerta de segurança, indicando que o site clonado não possui certificado HTTPS válido.
![image](https://github.com/user-attachments/assets/3e58c023-a0ca-41d4-a8ed-05b6f67ca538)
2) Os formulários não foram submetidos, com excessão do IE no Windows 7. O que sugere/indica que o Facebook utiliza tokens de autenticação CSRF e JS dinâmico, que não foram replicados pelo SET.
3) Em uma busca mais apurada sobre a segurança da rede social, há a indicação sobre utilização de headers de segurança, como CSP (Content-Security-Policy) e X-Frame-Options, que restringem onde e como seus recursos podem ser carregados - o que impede que partes importantes do site sejam carregados em sites clonados e justificam falhas de submissão de formulários, por exemplo.   





Até 31/12/2024 são essas as considerações. No mês de janeiro haverá novas tentativas de clonagem com alteração do HTML para tentar entregar o desafio com êxito de execução.



Feliz 2025!!!
