# Emitter il C#
Nova App

## Introduction Microsoft Intermediate Language (MSIL)
# 
Desenvolvimento de aplicações Desktop com il no Windows

## Get Started

### Executar o comando de criar pasta na linha de comando do Windows.

    C:\Users\ferna>mkdir Hello
    cd Hello
    
    
### Abrir o Visual Studio Code.

    Criar um projeto
    Arquivo > Novo Arquivo
    Nome do projeto : Hello
    Salvar
    
### Simples Hello World  

Alguns comandos il básicos são:
```
.assembly extern mscorlib {}
.assembly Hello {}
.module Hello.exe

.class Hello.Program
extends [mscorlib]System.Object
{
 .method static void Main(string[] args)
 cil managed
 {
  .entrypoint
  ldstr "Hello World"
  call void [mscorlib]System.Console::
  WriteLine(string)
  ret
 }
}
```
 
  

