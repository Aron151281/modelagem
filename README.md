# Modelagem - banco de dados MOD 3  
Criação de um projeto de banco de dados com exibição de modelagens para o armazenamento de informações 
sobre tecnologias utilizadas, empresas parceiras, áreas e colaboradores .

## Modelagem conceitual
![modelagem conceitual](https://github.com/Aron151281/modelagem/assets/132007858/c859d869-2333-4d14-88eb-89c5ac2424c2)


## Modelagem Lógica
![modelagem logica](https://github.com/Aron151281/modelagem/assets/132007858/f8055bdf-0e1b-4320-b752-c77580ce9d20)


O arquivo Excel disponível neste repositório contém a modelagem do banco de dados do sistema RESILIADATA. Ele inclui as seguintes tabelas e seus respectivos campos:

 ## Empresas Parceiras:

CNPJ (chave primária)
Nome
Endereço
Telefone
E-mail
Tecnologia_ID (chave estrangeira referenciando a entidade Tecnologia)
Tecnologia:

ID (chave primária)
Nome
Descrição
Área:

ID (chave primária)
Nome
Descrição
Empresa Parceira_CNPJ (chave estrangeira referenciando a entidade Empresa Parceira)
Tecnologia_Área:

ID (chave primária)
Tecnologia_ID (chave estrangeira referenciando a entidade Tecnologia)
Área_ID (chave estrangeira referenciando a entidade Área)
Colaborador:

CPF (chave primária)
Nome
Endereço
Telefone
E-mail
Empresa Parceira_CNPJ (chave estrangeira referenciando a entidade Empresa Parceira)
Área_ID (chave estrangeira referenciando a entidade Área)
Relacionamentos
Uma Empresa Parceira pode utilizar muitas Tecnologias (relação um para muitos).
Uma Empresa Parceira pode ter muitas Áreas (relação um para muitos).
Uma Área pode ter muitas Tecnologias (relação um para muitos).
Uma Tecnologia pode estar em várias Áreas (relação muitos para muitos).
Um Colaborador pode estar em apenas uma Empresa Parceira e apenas uma Área (relação um para um).
Exemplos de Registros
Aqui estão exemplos de registros para cada entidade:

## Empresas Parceiras:

CNPJ: 7677674647669, Nome: Brabus, Endereço: av  dajuda, 33 , Tel: (21) 9876-5432, E-mail: brabusa@kkk.com.br, Tecnologia_ID: 1
CNPJ: 123456789, Nome: biroliro@info, Endereço: rua do F, 987, Telefone: (11) 9997-0898, E-mail: bitoliro@info.com, Tecnologia_ID: 2
Tecnologia:

ID: 1, Nome: java, Descrição: Linguagem de programação versátil e de alto nível
ID: 2, Nome: python, Linguagem de consulta estruturada para bancos de dados relacionais
ID: 3, Nome: sql, Descrição: Linguagem de programação orientada a objetos
Área:

ID: 1, Nome: Webdev, Descrição: Desenvolvimento web e front-end, Empresa_Parceira_CNPJ: 7677674647669
ID: 2, Nome: Dados, Descrição: Ciência de dados e análise de informações, Empresa_Parceira_CNPJ: 123456789
Tecnologia_Área:

ID: 1, Tecnologia_ID: 1, Área_ID: 1
ID: 2, Tecnologia_ID: 1, Área_ID: 2
ID: 3, Tecnologia_ID: 2, Área_ID: 2
ID: 4, Tecnologia_ID: 3, Área_ID: 1
## Colaboradores:
CPF: 999999999, Nome: joão correa, Endereço: Rua itaipu, 444, Telefone: (12) 1111-1111, E-mail: joao@email.com, Empresa_Parceira_CNPJ: 123456789, Área_ID: 2
CPF: 22222222222, Nome: carlos andre , Endereço: travessa 3, 1111, Telefone: (46) 1111-1111, E-mail: carlos@email.com, Empresa_Parceira_CNPJ: 7677674647669, Área_ID: 1


# Tecnologias utilizadas :
Diagram,
Word

# Status : Finalizado

## Aron Augusto Bernardo Silva


