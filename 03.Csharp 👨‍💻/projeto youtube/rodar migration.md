
Abrir console: Clique em 'Tools' > 'Nuget package maneger' > 'Package manager console'

no default project selecionar o projeto 'Data'

comando no console para criar migration: add-migration CreateTableCourse (CreateTableCourse -> nome da migration)

comanod no console para atualizar o sql server depois de criar migration: update-database (para aparecer a tabela no sql server) 

ele vai criar uma pasta chamada 'Migrations' no projeto 'Data' com toda configuração que criamos de 'varchar(50)' etc..

Obs: para remover migration: Remove-Migration
Obs: no sql server ao criar migration ele cria uma tabela chama EFMalguma coisa, tem o historico das migrations ...