# Monitor Virtual USB — Guia de Instalação e Uso

Um utilitário simples para instalar e gerenciar um **monitor virtual no Windows**.
Indicado para desenvolvedores, streamers e usuários que precisam de uma tela extra para testes.

---

## 1. Requisitos

- Windows 7 / 8 / 10 / 11
- Permissões de Administrador
- .NET Framework instalado (padrão no Windows)

---

## 2. Instalação

### Passo 1 — Preparação

1. Baixe e extraia o projeto em uma pasta de sua preferência.
2. Abra o **Prompt de Comando (CMD)** como **Administrador**.
3. Navegue até a **pasta raiz do projeto**:

```cmd
cd "CAMINHO_DA_PASTA_RAIZ"
```

---

### Passo 2 — Instalar o Driver

Escolha o comando conforme a arquitetura do seu Windows:

#### Windows 32-bit (x86)

```cmd
deviceinstaller install usbmmidd.inf usbmmidd
```

#### Windows 64-bit (x64)

```cmd
deviceinstaller64 install usbmmidd.inf usbmmidd
```

---

## 3. Como Usar

### Ativar o Monitor Virtual

#### Windows 32-bit (x86)

```cmd
deviceinstaller enableidd 1
```

#### Windows 64-bit (x64)

```cmd
deviceinstaller64 enableidd 1
```

---

### Desativar o Monitor Virtual

#### Windows 32-bit (x86)

```cmd
deviceinstaller enableidd 0
```

#### Windows 64-bit (x64)

```cmd
deviceinstaller64 enableidd 0
```

---

## 4. Desinstalação Completa

### Windows 32-bit

```cmd
deviceinstaller stop usbmmidd
deviceinstaller remove usbmmidd
```

### Windows 64-bit

```cmd
deviceinstaller64 stop usbmmidd
deviceinstaller64 remove usbmmidd
```

---

## 5. Verificar se o Windows é 32 ou 64-bit

- Pressione **Win + Pause/Break** → veja o campo **Tipo de sistema**
- Alternativa: **Win + R → digite `winver` → Enter**

---

## 6. Notas Importantes

- Execute sempre o CMD como **Administrador**.
- Mantenha todos os arquivos do projeto na mesma pasta.
- Reinicie aplicativos (OBS, Discord etc.) após ativar/desativar o monitor.
- Recomenda-se criar backup antes de instalar drivers.

---

## 7. Solução de Problemas (Troubleshooting)

| Problema | Solução |
|---------|---------|
| **Acesso negado** | Execute o CMD como Administrador |
| **Driver não encontrado** | Verifique se está na pasta correta |
| **Monitor virtual não aparece** | Reinicie o aplicativo ou o Windows |
| **Comando não reconhecido** | Verifique se está na pasta raiz do projeto |

---

## 8. Suporte

Dúvidas e contato:
**@odorizzioficial**

---

## 9. Como contribuir

- Deixe uma **estrela** no repositório
- Compartilhe o projeto
- Inscreva-se no canal para apoiar o criador
