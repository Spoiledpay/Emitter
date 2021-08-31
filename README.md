# Flutter
Nova App

## Trabalhando com Flutter
# lagoon
A Scheme interpreter written in Rust

## Get Started

### Execute in interactive mode

    ./lagoon
    Doctor summary (to see all details, run flutter doctor -v):
    [√] Flutter (Channel stable, 2.2.3, on Microsoft Windows [versÃ£o 10.0.19042.1165], locale pt-BR)
    [√] Android toolchain - develop for Android devices (Android SDK version 30.0.3)
    [√] Chrome - develop for the web
    [√] Android Studio (version 4.1.0)
    [√] IntelliJ IDEA Community Edition (version 2021.2)
    [√] VS Code (version 1.59.1)
    [√] Connected device (2 available)
    
### Execute a Scheme script (extension does not matter)

    ./lagoon myscript.scm
    
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
