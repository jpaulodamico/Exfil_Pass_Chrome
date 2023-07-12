# Script de Exportação de Dados do Chrome

Este repositório contém um script de automação que recupera informações salvas no navegador Google Chrome, incluindo perfis de Wi-Fi e dados de login. Este script foi criado para demonstrar uma possível vulnerabilidade e deve ser usado apenas para fins educacionais. 

## ⚠️ Aviso Legal

Este script manipula dados sensíveis e pode ser usado de maneira mal-intencionada se cair em mãos erradas. Este código é fornecido apenas para fins educacionais e de conscientização. Nunca use este código sem o consentimento explícito do proprietário do computador onde ele está sendo executado.

## 🎯 Objetivo

O objetivo deste script é demonstrar como os dados armazenados localmente no navegador Google Chrome podem ser facilmente recuperados por um invasor com acesso físico ao computador.

## 🔍 Como funciona

O script executa os seguintes passos:

1. Abre o PowerShell com privilégios administrativos.
2. Navega para a raiz do diretório `C:\` e cria uma nova pasta chamada `l`.
3. Exporta todos os perfis de Wi-Fi salvos no computador, incluindo as chaves de segurança, para a pasta `l`.
4. Desativa o Windows Defender e a política de execução de scripts do PowerShell para permitir a execução do próximo script.
5. Copia os arquivos `Login Data` e `Local State` do diretório de dados do usuário do Chrome para a pasta `l`.
6. Baixa e executa um script do PowerShell de uma URL do Dropbox. Este script deve ser um script que manipula os dados copiados conforme necessário (por exemplo, enviando-os por e-mail para um endereço especificado).
7. Remove a pasta `l` e todos os seus conteúdos.
8. Fecha o PowerShell.

## 🚀 Como executar

1. Salve o conteúdo do script em um arquivo `.txt`.
2. Abra o aplicativo DuckEncoder e selecione o arquivo `.txt` criado na etapa anterior.
3. Clique no botão "Encode" para criar um script `inject.bin`.
4. Copie o script `inject.bin` para a raiz do seu USB Rubber Ducky.
5. Insira o USB Rubber Ducky no computador de destino.

## 📄 Licença

Este projeto é licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
