# Como configurar/instalar/usar o `whois` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar o `whois` no `Linux Ubuntu`.

## _Abstract_

_In this document are contained the main commands and settings to set up/install the `whois` on `Linux Ubuntu`._


## Descrição [2]

### `whois`

O `"whois"` é um protocolo e uma ferramenta de linha de comando utilizada para consultar informações sobre registros de domínio na Internet. Ele permite aos usuários obter detalhes sobre a propriedade, registros de nome, data de registro, data de expiração e informações de contato associadas a um determinado domínio. Essas consultas são realizadas em bancos de dados distribuídos, mantidos por registradores de domínios e autoridades de registro, e fornecem transparência e visibilidade sobre a propriedade e a gestão de domínios na Internet. O `"whois"` é frequentemente utilizado por administradores de rede, proprietários de domínios, pesquisadores de segurança e profissionais de TI para investigar questões relacionadas a nomes de domínio, como verificar a disponibilidade de um domínio, identificar informações de contato do proprietário de um domínio ou investigar atividades suspeitas na Internet.

### `DNS`

O DNS, ou Sistema de Nomes de Domínio, é um sistema fundamental na Internet que traduz nomes de domínio legíveis por humanos, como exemplo.com, em endereços IP numéricos, que são utilizados pelos computadores para localizar serviços e recursos na rede. Funcionando como uma espécie de catálogo telefônico da Internet, o DNS permite que os usuários acessem sites, enviem e recebam e-mails, e realizem outras atividades online, sem precisar memorizar endereços IP complexos. Quando um usuário digita um nome de domínio em um navegador da web ou em outro aplicativo de Internet, o computador faz uma consulta DNS para encontrar o endereço IP correspondente associado a esse nome de domínio. Esse processo envolve a comunicação com servidores DNS distribuídos em toda a Internet, começando com servidores de nomes raiz e percorrendo uma hierarquia de servidores DNS autorizados até encontrar a resposta desejada. O DNS é essencial para o funcionamento da Internet moderna e é uma parte crítica da infraestrutura de rede global.


## 1. Como configurar/instalar/usar o `whois` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `whois` no `Linux Ubuntu`, você pode seguir estes passos:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Suft + Alt + T`

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

3. O `whois` já vem pré-instalado do `Linux Ubuntu`. Sendo assim, caso NÃO esteja instalado, para instalar o `whois` tanto no `Linux Ubuntu` quanto no `Linux Ubuntu`, siga as instruções abaixo:

Para configurar/instalar/usar o `whois` no `Linux Ubuntu`, você pode seguir estes passos:

4. **Execute o comando:** `sudo apt install whois -y`

## 2. Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `whois` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt autoclean                     
    sudo apt autoremove
    sudo apt update -y
    sudo apt autoremove
    sudo apt autoclean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install whois
    whois meklogistics.com.br
    ```


## Referências

[1] OPENAI. ***Instalar `whois` no ubuntu.*** Disponível em: <https://chat.openai.com/c/b5da860f-1627-4f20-9fc7-a063b9248c5b> (texto adaptado). Acessado em: 09/02/2024 00:37.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). Acessado em: 09/02/2024 00:37.

[3] USER: FREE EDUCATION FOR ALL. ***Lesson 29: whois.*** Disponível em: <https://www.youtube.com/watch?v=FYJ7oiiYvek&list=PLnjNR4-S-EVqfJWovxEJyb7I0IOkKkoYM&index=29> (texto adaptado). Acessado em: 09/02/2024 00:37.

