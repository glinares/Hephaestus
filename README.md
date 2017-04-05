 # Hephaestus
Open Source Office Malware Generation & Polymorphic Engine for Red Teams and QA testing


# Update April 4th, 2017
Current list of implemented Features in Hephaestus as of April 4th, 2017:

# Polymorphic Engine Features:

  - Randomized Variables & Functions Names  
    Standard procedure randomized variables and functions 
    
  - Anti-Entropic Variable Generation  
    Using commonly used (US-language) variables in typical business VBA modules to name variables & functions to avoid randomized variable detection.
    
  - VBA Constant String Building  
    String and characters can be generated from string constants in VBA to avoid using string variables.

  - VBA Constant Numeric Substitution  
    Static numbers used in VBA can be substituted with VBA constants to prevent the display of any number.
  
  - Automatic Numeric Factoring  
    Used to break down numbers into factors to hinder reverse engineering and analysis.  This can be combined with the use of Numeric Constant Substitutions to further increase time to reverse engineer.
    
  - Multiple VBA Numeric Obfuscation Schemes  
  Using built in VBA functions to obfuscate numeric values from being displayed or to complicate their analysis
    
  - String value obfuscations  
  Currently only very basic string obfuscation code has been added.  I will be adding a ton of new obfuscation methods to obfuscate strings, including a string building system.
  
  - Garbage Code Generator  
    Various types of garbage code styles to inject into functions.
  
  - Error Handler Code Flow Obfuscation  
    Abusing Error Handlers to obfuscate code flow and insertion of garbage code
  
# Anti-Analysis Methods:

  - Multiple Sandbox Detection Algorithms  
    Various methods to detect sandboxes and virtualized environments
    
  - Anti-Analysis tool and Process Detection  
    Configurable list of tools and processes to detect.
    
  - VBA IDE (VBE) Detection  
    Detects the VBA IDE Window being active
    
  - Breakpoint Deletion  
    Will delete all the current breakpoints established in the VBA IDE (VBE) environment.
    
  - Step Debugging Detection  
    Can detect if a user is stepping through code using several methods.
    
  - Counter-Step Debugging  
    Multiple methods to prevent code stepping from occurring.
    
  - Domain / Environment Targeting  
    Execute only if specific domain / environment conditions occur.
    
  - Encrypted Application.Variable Storage  
    Will support Application.Variable storage for strings, numbers, functions, and variables.  
    This prevents tools from dumping your code and doing static analysis on your code.
    
  - Environment Fingerprinting  
    Will take snapshot of various system properties and store them in Application.Variables to determine if execution
    environment has changed widely since last execution.
    
  - Application.Variable Self-Destruct  
    Will delete all variables and its code functions upon detecting a sandbox, analysis, or different environment than last
    executed.
    
  - "Detected Mode" Payload  
    Will execute a backup payload (such as cryptolocker download/exec) post detection to feign actual purpose
    
   
    
# Payload Delivery Methods  
  - PowerShell
  - Generate .NET Binary & Compile with MSBuild
  - Binary Extraction & Execution
  - Python (Mac OSX)
  - System Command Execution
  - Download File & Execute
  
    
    
    
 # Researching  
  - C2 Server Timer Events  
    Has the ability to send C2 server timer events which can be used to identify analysis and/or multiple executions
    
  - C2 Hosted Application.Variables  
    Has the ability to request C2 for variables for strings, numbers, functions, and variables, thus only partial code in Macro form.
  
  

  
