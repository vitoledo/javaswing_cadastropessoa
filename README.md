## Estrutura do Código

### 1.Importações
```java
import javax.swing.*;
import java.awt.*;
```
Importa os pacotes necessários para criação de janelas (swing) e gerenciamento de layout (awt).

### 2.Classe Principal: CadastroPessoa
A classe herda `JFrame`, o que transforma a classe em uma janela GUI

### 3.Componentes da Interface
São declarados como variáveis privadas:
- `JTextField` para entrada de texto.
- `JComboBox` para seleção entre pessoa física ou jurídica.
- `JCheckBox` para marcar se a pessoa é fornecedora.
- `JRadioButton` e `ButtonGroup` para indicar a situação (ativo/inativo).

### 4.Construtor: CadastroPessoa()
Responsável por montar toda a interface:
- Define tamanho, título, layout, cor de fundo.
- Adiciona rótulos (`JLabel`) e campos de texto (`JTextField`).
- Posiciona manualmente os componentes usando `setBounds()`.
- Usa `add()` para adicionar componentes ao JFrame.
- Define o botão “Confirmar”, que mostra uma mensagem de sucesso e limpa os campos.
- Define os botões “Excluir” e “Limpar”, que também apagam os dados do formulário.

### 5.Botões e Ações
- **Confirmar**: Exibe `JOptionPane` com mensagem de sucesso e limpa os campos.
- **Excluir**: Apenas limpa os campos (mesmo efeito de "limpar").
- **Limpar**: Limpa todos os campos do formulário.

