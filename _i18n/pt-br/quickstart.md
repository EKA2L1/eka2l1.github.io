Utilize o *Índice* à direita para acessar a seção de que você precisa.

# Requisitos

## Para a versão de PC:

### Mínimo

- **Sistema Operacional:** Precisa ser **de 64 bits**. Para **Windows**, você deve ter a partir do *Windows 7* ou superior
- **Processador:** Qualquer CPU de 64 bits fabricada por volta de 2007, a partir do modelo **Core 2 Duo E4300**
- **Memória:** 2 GB de RAM no mínimo
- **Placa gráfica:** Qualquer GPU compatível com OpenGL 3.1 ou superior

### Recomendado

- **Sistema Operacional:** Precisa ser **de 64 bits**. Para **Windows**, é recomendado usar o *Windows 10*
- **Processador:** Qualquer CPU Intel ou AMD com 4 núcleos ou superior
- **Memória:** 4 GB de RAM ou mais
- **Placa gráfica:** Qualquer GPU compatível com OpenGL 3.3 ou superior

## Para a versão de Android:


### Mínimo

- **Sistema Operacional:** Android 5.0 de 32 bits
- **Processador:** Qualquer CPU ARMv7 ou superior. **ARMv6 e inferiores não são suportados!**
- **Memória:** 2 GB de RAM no mínimo
- **Placa gráfica:** Qualquer GPU compatível com OpenGL ES 3.0 ou superior

### Recomendado
- **Sistema Operacional:** Android 7.0 de 64 bits (32 bits está em fase experimental)
- **Processador:** CPU ARMv8
- **Memória:** 4 GB de RAM ou mais
- **Placa gráfica:** Qualquer GPU compatível com OpenGL ES 3.2 ou superior

# Instalação
## Você precisará de:
- ROM (De qualquer dispositivo Symbian, exemplos: N-Gage, Nokia N97, Nokia E5)
- Os arquivos do drive Z (do mesmo dispositivo do qual a ROM foi dumpeada). Consulte a [seção](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) específica
  da Wiki para aprender a como dumpear uma ROM você mesmo

## Configuração:
- Baixar [EKA2L1](https://12z1.com/download/)
- Você pode iniciar o EKA2L1 diretamente e interagir com o emulador por meio da GUI, ou interagir diretamente por meio da linha de comando.
- Use --help para ver a lista de comandos disponíveis (se você quiser interagir com o emulador por meio de comandos)
- Instale um novo dispositivo através de Files/Install device
  
## Instalação de um novo dispositivo no EKA2L1
- EKA2L1 tem uma GUI para instalar um novo dispositivo. Com a GUI, vá Files/Install device
  ![Installdevice](https://camo.githubusercontent.com/08fa49e5578f4045abc98a0cec22bd4bb8cc52480eb3ffab5ed3bee28f7b0e0c/68747470733a2f2f6d656469612e646973636f72646170702e6e65742f6174746163686d656e74732f3536353139363435373433353539343735352f3730303235303631373233383635303937312f756e6b6e6f776e2e706e67)
- Esta interface irá guiá-lo durante a instalação. Se uma **falha repentina** aparecer ou o **dispositivo reverter a instalação** devido a **motivos de falsificação**, **entre em contato com o desenvolvedor** para suporte e correções, se necessário.
  - Se a instalação falhar porque a **determinação da versão Symbian falhou**, você também deve entrar em contato com um desenvolvedor para ajudar o emulador a melhorar este processo
  
## Alterar diretório de dados::
- EKA2L1 tenta armazenar dados em uma única pasta. Por padrão, é uma pasta chamada "dados" no mesmo diretório do executável. Você pode alterar o caminho por meio da GUI File/Preferences ou alterá-lo em **config.yml** com a chave **data-storage**
  - Observe que isso **não move** a pasta de dados. Você mesmo tem que movê-la manualmente (Copiar e Colar)
