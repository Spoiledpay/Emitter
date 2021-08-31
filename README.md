# Flutter
Nova App

## Trabalhando com Flutter
# https://flutter.dev/docs/get-started/install/windows
Desenvolvimento de aplicações mobile com Flutter no Windows

## Get Started

### Executar o comando de verificação na linha de comnando do Windows.

    C:\Users\ferna>flutter doctor
    Doctor summary (to see all details, run flutter doctor -v):
    [√] Flutter (Channel stable, 2.2.3, on Microsoft Windows [versÃ£o 10.0.19042.1165], locale pt-BR)
    [√] Android toolchain - develop for Android devices (Android SDK version 30.0.3)
    [√] Chrome - develop for the web
    [√] Android Studio (version 4.1.0)
    [√] IntelliJ IDEA Community Edition (version 2021.2)
    [√] VS Code (version 1.59.1)
    [√] Connected device (2 available)
    • No issues found!
    
### Aprovar as licenças do Android.

    flutter doctor --android-licenses
    
### Embed Lagoon in Rust application  
  
    pub mod scheme;

    use scheme::interpreter::Interpreter;

    fn main() {
        // Create an interpreter object
        let mut interp = Interpreter::new();
        
        // Evaluate the expressions represented by a string
        interp.eval_string("(+ 1 2 3)");
                
        // Run interpreter in REPL mode
        interp.run_repl();
    }
