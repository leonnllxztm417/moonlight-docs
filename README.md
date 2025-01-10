# Moonlight Documentation
This repository is the home of [our wiki](https://github.com/moonlight-stream/moonlight-docs/wiki).
monlight_vpc/
├── monlight_vpc.py
├── README.md
├── .gitignore
└── requirements.txt
class VirtualPC:
    def __init__(self):
        self.system_status = "on"
        self.memory = 4  # GB
        self.disk_space = 100  # GB
        self.installed_apps = ["Terminal", "Web Browser", "File Explorer"]
    
    def show_status(self):
        print(f"PC Status: {self.system_status}")
        print(f"Memory: {self.memory} GB")
        print(f"Disk Space: {self.disk_space} GB")
    
    def list_apps(self):
        print("Installed Applications:")
        for app in self.installed_apps:
            print(f"- {app}")
    
    def shut_down(self):
        self.system_status = "off"
        print("Shutting down the PC...")

    def start(self):
        self.system_status = "on"
        print("Starting the PC...")

def main():
    pc = VirtualPC()
    print("Welcome to Monlight Virtual PC!")
    
    while True:
        print("\nWhat would you like to do?")
        print("1. Show system status")
        print("2. List installed applications")
        print("3. Shut down")
        print("4. Start PC")
        print("5. Exit")
        
        choice = input("Enter your choice: ")
        
        if choice == "1":
            pc.show_status()
        elif choice == "2":
            pc.list_apps()
        elif choice == "3":
            pc.shut_down()
        elif choice == "4":
            pc.start()
        elif choice == "5":
            print("Goodbye!")
            break
        else:
            print("Invalid choice. Please try again.")

if __name__ == "__main__":
    main()
    # Monlight Virtual PC

Este é um projeto simples de simulação de um PC virtual, onde você pode interagir com um sistema básico em um terminal. O projeto simula um PC com funcionalidades como verificar status, listar aplicativos e ligar/desligar o sistema.

## Funcionalidades

- Verificar status do sistema (ligado/desligado, memória e espaço no disco).
- Listar aplicativos instalados.
- Ligar e desligar o PC.

## Como rodar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/monlight-vpc.git
   cd monlight-vpcpython monlight_vpc.py
   
### Passo 4: Adicionando um arquivo `.gitignore`
Esse arquivo é utilizado para garantir que arquivos desnecessários não sejam enviados para o GitHub. Crie o arquivo `.gitignore` com o seguinte conteúdo:

#### `.gitignore`
```gitignore
*.pyc
__pycache__
git clone https://github.com/seu-usuario/monlight-vpc.git
cd monlight-vpc
git add .
git commit -m "Primeiro commit do Monlight Virtual PC"
git push origin main
