ℹ️ Notice: This README is written in Brazilian Portuguese (pt-br).

# Desafio DevOps

O objetivo deste desafio é avaliar sua habilidade em configurar, gerenciar e otimizar infraestruturas na nuvem, bem como sua capacidade de implementar práticas contínuas de integração e entrega (CI/CD). Você trabalhará com a AWS, para hospedar um site estático e automatizar o seu processo de deploy.

Se você ainda não possui uma conta na AWS, crie uma conta gratuita. Tenha em mente as limitações do plano gratuito ao criar e configurar recursos.

## **Teste 1 - Criar e Configurar uma Instância EC2:**

- Suba uma instância EC2 usando a AMI do Ubuntu Server 22.04 LTS.
- Configure a instância para uso com um par de chaves SSH (arquivo PEM) e defina as regras de segurança do grupo de segurança (Security Group) para permitir o tráfego HTTP e SSH.
- Instale e configure um servidor web (Nginx ou Apache) na instância EC2. Garanta que a página padrão do servidor web seja acessível publicamente através do IP da instância.

## **Teste 2 - Criar um bucket no S3 para servir um site estático**

1. **Criar um Bucket no S3:**
    - Crie um bucket no S3 para armazenar os arquivos do seu site estático.
    - Configure o bucket para hospedar um site estático, e habilite o acesso público (lembre-se de aplicar as melhores práticas de segurança).
2. **Hospedar um Site Estático:**
    - Crie uma página HTML simples que sirva como a página inicial do seu site.
    - Faça upload dos arquivos do site para o bucket do S3 e configure o bucket para usar o arquivo HTML como página inicial.

## Teste 3 - **Esteira de Deploy Automatizado com GitHub Actions**

1. **Repositório GitHub:**
    1. Crie um repositório no GitHub para armazenar o código do seu site estático.
2. **Configurar GitHub Actions:**
    1. Configure uma esteira de CI/CD usando GitHub Actions para automatizar o deploy do site estático.
    2. O workflow deve detectar mudanças na branch principal e fazer o deploy dos arquivos no bucket S3 e na instância EC2 configurados anteriormente.

## **Entrega do Desafio**

- Documente todos os passos realizados, incluindo:
    - Comandos utilizados para configurações e instalações.
    - Capturas de tela da instância EC2 funcionando, do site estático hospedado no S3 acessível publicamente, e do GitHub Actions executando o pipeline de CI/CD.
- Compartilhe o código do seu site estático e os arquivos de configuração do GitHub Actions no repositório do GitHub.
- Envie o link do repositório junto com a documentação para a análise.