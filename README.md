# Configuração de Instância EC2 com Python e Streamlit  

Este repositório documenta os passos e o código utilizado para configurar uma instância EC2 na AWS, obter acesso root, definir uma senha para o root e configurar um ambiente para rodar um aplicativo básico com Streamlit, incluindo a renderização de uma imagem armazenada no S3.

---

## 📋 Passos Realizados  

### 1. **Configuração da Instância EC2**
- Criar uma instância EC2 na AWS (Amazon Linux 2).
- Configurar o Security Group com regras para:
  - Acesso SSH (porta 22)
  - Acesso HTTP (porta 80)
  - Outras portas conforme a necessidade.

### 2. **Acesso Root**  
- Conectar na instância EC2 via SSH:  
  ```bash
  ssh -i "meu-arquivo.pem" ec2-user@<IP_DA_INSTÂNCIA>
