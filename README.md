# Atividade com monitoramento Nginx - Compass UOL | Atividade Prática 1 #PB - Novembro 2024 | DevSecOps
Atividade devsecops - Linux e AWS na prática

Instalação do WSL no Windows

Para instalar o WSL (Subsistema do Windows para Linux) no Windows, siga o guia abaixo. Certifique-se de que seu sistema operacional seja Windows 10 (versão 2004 ou superior) ou Windows 11.

2. Ative o WSL
Abra o Prompt de Comando ou PowerShell como administrador.
Clique com o botão direito no menu Iniciar e escolha Prompt de Comando (Admin) ou Windows PowerShell (Admin).
Digite o seguinte comando e pressione Enter:

wsl --install

Este comando:
Ativa os componentes necessários do WSL.
Instala a última versão do WSL 2.

3. Reinicie o computador
Após a execução do comando acima, reinicie seu computador se solicitado.

4. Escolher uma Distribuição Linux:
Após reiniciar o sistema, acesse a Microsoft Store e selecione uma distribuição Linux, como o Ubuntu 20.04 LTS.
Configuração Inicial do WSL:
Após a instalação, abra a distribuição Linux instalada (como o Ubuntu) e configure o nome de usuário e senha para o ambiente Linux.

Após atualizar o Sistema WSL:
No terminal da distribuição Linux (por exemplo, Ubuntu), execute os seguintes comandos para atualizar:

sudo apt update
sudo apt upgrade
