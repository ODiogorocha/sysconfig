# Guia de Instalação de Ferramentas no macOS via Terminal

Este guia contém os comandos necessários para instalar as seguintes ferramentas no macOS: iTerm2, Oh My Zsh, Python, Java, Lua, linguagens de programação (C, C++, C#), engines (Godot e Unity), MySQL e MySQL Workbench, utilizando o **Homebrew** como gerenciador de pacotes.

---

## 1. **Instalando o Homebrew**
O Homebrew é um gerenciador de pacotes essencial para instalar ferramentas no macOS.

### Passos:
1. Instale o Homebrew:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. Verifique se a instalação foi bem-sucedida:
   ```bash
   brew --version
   ```

---

## 2. **Instalando o iTerm2**
O iTerm2 é uma alternativa avançada ao terminal padrão do macOS.

### Passos:
1. Instale o iTerm2:
   ```bash
   brew install --cask iterm2
   ```
2. Abra o iTerm2 diretamente:
   ```bash
   open -a iTerm
   ```

---

## 3. **Instalando o Oh My Zsh**
O Oh My Zsh é uma ferramenta para gerenciar a configuração do shell Zsh.

### Passos:
1. Certifique-se de que o Zsh é o shell padrão (o macOS já utiliza Zsh por padrão em versões recentes):
   ```bash
   echo $SHELL
   ```
2. Instale o Oh My Zsh:
   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```
3. Reinicie o terminal para aplicar as alterações.

---

## 4. **Instalando o Python**
O macOS já vem com uma versão do Python, mas para instalar a versão mais recente:

### Passos:
1. Instale o Python:
   ```bash
   brew install python
   ```
2. Verifique a instalação:
   ```bash
   python3 --version
   pip3 --version
   ```

---

## 5. **Instalando o Java**
### Passos:
1. Instale o OpenJDK:
   ```bash
   brew install openjdk
   ```
2. Configure o Java no sistema:
   ```bash
   sudo ln -sfn /usr/local/opt/openjdk/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk.jdk
   ```
3. Verifique a instalação:
   ```bash
   java --version
   ```

---

## 6. **Instalando o Lua**
### Passos:
1. Instale o Lua:
   ```bash
   brew install lua
   ```
2. Verifique a instalação:
   ```bash
   lua -v
   ```

---

## 7. **Instalando o C e C++**
O Xcode Command Line Tools inclui os compiladores para C e C++.

### Passos:
1. Instale as ferramentas de linha de comando do Xcode:
   ```bash
   xcode-select --install
   ```
2. Verifique a instalação:
   ```bash
   gcc --version
   g++ --version
   ```

---

## 8. **Instalando o C#**
Para C#, instale o .NET SDK da Microsoft.

### Passos:
1. Instale o .NET SDK:
   ```bash
   brew install --cask dotnet-sdk
   ```
2. Verifique a instalação:
   ```bash
   dotnet --version
   ```

---

## 9. **Instalando o Godot**
### Passos:
1. Instale o Godot usando o Homebrew:
   ```bash
   brew install --cask godot
   ```
2. Abra o Godot:
   ```bash
   open -a Godot
   ```

---

## 10. **Instalando o Unity**
### Passos:
1. Baixe o Unity Hub:
   ```bash
   brew install --cask unity-hub
   ```
2. Abra o Unity Hub:
   ```bash
   open -a "Unity Hub"
   ```

---

## 11. **Instalando o MySQL**
### Passos:
1. Instale o MySQL:
   ```bash
   brew install mysql
   ```
2. Inicie o serviço do MySQL:
   ```bash
   brew services start mysql
   ```
3. Acesse o MySQL:
   ```bash
   mysql -u root -p
   ```

---

## 12. **Instalando o MySQL Workbench**
### Passos:
1. Instale o MySQL Workbench:
   ```bash
   brew install --cask mysqlworkbench
   ```
2. Abra o MySQL Workbench:
   ```bash
   open -a "MySQL Workbench"
   ```

---

## Conclusão
Agora você tem todas as ferramentas instaladas e configuradas no macOS. Caso tenha problemas ou dúvidas durante o processo, revise os comandos ou consulte a documentação oficial de cada ferramenta.
