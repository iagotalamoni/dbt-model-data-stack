Passos de configuração:

-> Editar o arquivo project
  -> O nome do arquivo é dbt_project.yml <br>
  -> Alteramos o campo name (linha 5); o profile (linha 11); se atentar para mudar a linha 36 com o nome do prjeto (o que colocou na linha 5)

-> Criar o arquivo de profile
  -> Pegamos um template e colocamos as informações do banco de dados

-> Criar os modelos base
  -> As nomenclaturas do sql no dbt são diferentes
  -> Como criamos um modelo? Tudo que jogarmos na pasta models vira um modelo (é refletido no DW)
  -> o arquivo schema.yml é utilizado para "explicar" para o dbt o que são os modelos

-> Criar o modelo relacionado
  -> Utilizamos os modelos base para fazer joins e criar uma tabela com todas as informações que queremos
  -> no from temos o source (ele foi declarado no arquivo schema.yaml)

-> Criar o schema

-> Testar execução

-> Conferir transformação no DW
