## 🛠️ Dll-Com32-CalculoQuartil
Componente DLL de cálculo e estatísticas e quadro de quartil em C# .NET para ser utilizado como componente COM.

#### 📋 O que você vai encontrar neste projeto
| Tecnologia | Descrição |
|-----------|-----------|
| **DLL** | Criação de DLL em Csharp |
| **FoxPro** | Utilização do uso como componente DLL e consumindo dados retornados em formato Json.|
| **Json** |Serialização e desserialização utilizado nas linguaguens |
| **COM** | Criação de Componente Objetos COM/ActiveX em .NET onde para ser usadas por outras linguaguens (rundll32), devem ter e serem criadas como ComVisible(true) e serem registradas para interoperação com registro (regasm.exe). |

#### Requisitos do Projeto
A DLL deve ser registrada com o seguinte .BAT, necessário ajustar o diretório do arquivo BAT.
```bash
@ECHO OFF
echo %cd%
C:\Windows\Microsoft.NET\Framework\v4.0.30319\RegAsm.exe D:\DLLTeste3\DLLTeste3\Foxpro\DLLTeste3.dll /codebase /tlb
C:\Windows\Microsoft.NET\Framework64\v4.0.30319\RegAsm.exe D:\DLLTeste3\DLLTeste3\Foxpro\DLLTeste3.dll /codebase /tlb
timeout /t 20
EXIT
```

#### Cálculo do Quartilo que é ?
Os quartis são medidas estatísticas que dividem um conjunto de dados ordenados (do menor para o maior) em quatro partes iguais, cada uma contendo 25% dos dados. Eles são fundamentais para entender a distribuição e a dispersão dos dados, indo além do que uma simples média pode mostrar.
