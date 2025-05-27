# lab-summary
This repository contains a summary of lessons learned during the development of the laboratory at DIO.

## Resumo
O Portal Azure oferece uma interface gráfica intuitiva para a criação e gestão de VMs. Este guia foca na criação de uma VM com Windows Server 2022, conexão via RDP (Remote Desktop Protocol) e instalação opcional do servidor web IIS para teste.

1 - **Detalhes da Instância:**
- Defina um Nome da máquina virtual (ex: minhaVM).
- Escolha uma Imagem (ex: Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2).
- Mantenha as outras configurações padrão ou ajuste conforme necessário (Região, Zona de Disponibilidade, etc.)
   
2 - **Conta de Administrador:**
- Crie um Nome de usuário (ex: usuarioazure).
- Defina uma Senha segura (mínimo 12 caracteres, atendendo aos requisitos de complexidade).
  
3 - **Regras de Porta de Entrada:**
- Selecione "Permitir portas selecionadas".
- Habilite as portas RDP (3389) para acesso remoto e HTTP (80) se planeja hospedar um servidor web.
- Revisão e Criação: Revise as configurações e clique em "Examinar + criar" e, após a validação, em "Criar".
- Acesso ao Recurso: Após a implantação ser concluída, clique em "Ir para o recurso".

### Conectando-se à VM via RDP
1. Na página de visão geral da VM, vá em Conectar > RDP.
2. Mantenha as opções padrão e clique em Baixar arquivo RDP.
3. Abra o arquivo .rdp baixado.
4. Clique em Conectar.
5. Na janela de segurança, selecione Mais opções > Usar uma conta diferente.
6. Digite o nome de usuário como localhost\<seu_nome_de_usuario> (substitua <seu_nome_de_usuario> pelo que você definiu).
7. Insira a senha criada.
8. Clique em OK e aceite eventuais avisos de certificado clicando em Sim ou Continuar.
