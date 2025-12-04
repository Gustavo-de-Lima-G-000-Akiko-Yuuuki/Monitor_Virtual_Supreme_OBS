# Monitor Virtual USB

Um utilitário simples para instalar e gerenciar um **monitor virtual no Windows**.  
Ideal para desenvolvedores, streamers e usuários que precisam de um monitor adicional para testes.

---

## 📢 Apoie o Projeto
Inscreva-se no canal para ajudar <3 **#Rumo100K**  
Siga nas redes sociais: **@odorizzioficial** <3

---

## 📋 Requisitos

- Windows 7 / 8 / 10 / 11  
- Permissões de Administrador  
- .NET Framework (geralmente já instalado no Windows)

---

## 🚀 Instalação

### **Passo 1: Preparação**

1. Baixe e extraia o projeto para uma pasta de sua preferência.  
2. Abra o **CMD (Prompt de Comando)** como Administrador.  
3. Navegue até a pasta raiz do projeto:

```cmd
cd "CAMINHO_DA_PASTA_RAIZ"
Substitua "CAMINHO_DA_PASTA_RAIZ" pelo diretório onde o projeto foi extraído.

Passo 2: Instalar o Driver
Execute um dos comandos abaixo de acordo com a arquitetura do seu Windows:

Para sistemas 32-bit (x86):
cmd
Copiar código
deviceinstaller install usbmmidd.inf usbmmidd
Para sistemas 64-bit (x64):
cmd
Copiar código
deviceinstaller64 install usbmmidd.inf usbmmidd
🖥️ Como Usar
Ativar Monitor Virtual
32-bit (x86):
cmd
Copiar código
deviceinstaller enableidd 1
64-bit (x64):
cmd
Copiar código
deviceinstaller64 enableidd 1
Desativar Monitor Virtual
32-bit (x86):
c
Copiar código
deviceinstaller enableidd 0
64-bit (x64):
cmd
Copiar código
deviceinstaller64 enableidd 0
🗑️ Desinstalação
Para sistemas 32-bit (x86):
cmd
Copiar código
deviceinstaller stop usbmmidd
deviceinstaller remove usbmmidd
Para sistemas 64-bit (x64):
cmd
Copiar código
deviceinstaller64 stop usbmmidd
deviceinstaller64 remove usbmmidd
🔍 Como verificar se seu Windows é 32 ou 64-bit
Pressione Win + Pause/Break

Veja o campo "Tipo de sistema":

Sistema operacional de 64 bits → use comandos 64-bit

Sistema operacional de 32 bits → use comandos 32-bit

Alternativa:
Pressione Win + R, digite winver e pressione Enter.

⚠️ Notas Importantes
Execute sempre o CMD como Administrador

Mantenha todos os arquivos do projeto na mesma pasta

Reinicie aplicativos (OBS, Discord etc.) após ativar/desativar o monitor

Faça backups antes de instalar drivers

❓ Troubleshooting (Solução de Problemas)
Problema	Solução
Erro de acesso negado	Execute o CMD como Administrador
Driver não encontrado	Verifique se está na pasta correta
Monitor não aparece	Reinicie o aplicativo ou o Windows
Comando não reconhecido	Verifique se está na pasta raiz do projeto

📞 Suporte
Em caso de dúvidas ou problemas, entre em contato pelas redes sociais:
@odorizzioficial

⭐ Contribuição
Se este projeto foi útil para você:

⭐ Dê uma estrela no repositório

📢 Compartilhe com amigos

🎥 Inscreva-se no canal

Agradecimentos especiais a todos os apoiadores!
Mais tutoriais e ferramentas úteis no canal! 🚀
