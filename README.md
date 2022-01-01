      IaC (Infreestrutura como Código)

- Na AWS em "Instâncias > Tipos de instância" podemos ver as AMIs(Imagens) disponíveis para as máquinas;

- Já em "Imagens => AMI Catalog" podemos escolher a AMI e copiar o código AMI para gerar a máquina pelo terraform (A AMI muda por região)

- Idempotência => É quando se chama uma funcionalidade varias vezes com o mesmo valor, e o resultado é sempre o mesmo

---

## TERRAFORM (https://www.terraform.io/)
 
 Com o Terraform podemos escrever nossos scripts de infraestrutura

 1. Criar arquivo main.tf
 2. Colar o conteúdo disponível no site do terraform
 3. Instalar o AWS CLI pelas instruções do site da AWS
 4. Baixar as chaves em IAM
 5. Configurar as chaves no comando "aws configure"
 6. Criar par de chaves em "EC2 -> Rede e Segurança -> Par de chaves"
 7. Colocar a chave dentro da pasta onde está o main.tf
 8. Associar a chave no arquivo main.tf na tag resource -> key_name;

## ANSIBLE
 
 Permite automatizar a isntalação e atualização de algumas ferramentas;

---

    terraform init
   Iniciar as configurações do terraform

    terraform plan
   Vai mostrar planejamento

    terraform apply
   Vai aplicar o planejamento IaC
