
1. @Component: Uma anotação genérica para qualquer componente gerenciado pelo Spring.

2. @Configuration: Ela indica que a classe possui métodos de configuração do Spring e que os beans retornados por esses métodos devem ser gerenciados pelo container do Spring.

3. @Bean: Usada em métodos dentro de uma classe marcada com @Configuration para definir um bean Spring.

4. @Service: Indica que a classe marcada é um serviço e pode conter a lógica de negócios. É uma especialização da anotação @Component.

5. @Repository: Especifica que a classe é um repositório, uma abstração de acesso a dados. Também é uma especialização da anotação @Component.

6. @Autowired: Permite a injeção automática de dependências. O Spring resolve e injeta beans colaboradores no seu bean.

7. @RequestMapping: Usada para mapear solicitações web para métodos específicos nos controllers. Pode ser usada tanto no nível da classe quanto do método.

8. @RestController: Usada em classes para indicar que a classe é um controller e que todos os métodos retornam um objeto de domínio ao invés de uma view. É uma combinação das anotações @Controller e @ResponseBody.

9. @PathVariable: Usada para extrair valores de variáveis do URI de uma solicitação web e passá-las como parâmetros para os métodos de controller.

10. @RequestParam: Usada para acessar os parâmetros da solicitação web. Permite que você mapeie parâmetros de solicitações GET ou POST para os parâmetros do seu método.

11. @RequestBody: é usada em métodos de controllers para indicar que o corpo da requisição HTTP deve ser convertido automaticamente em um objeto Java. É comumente usada em APIs REST para lidar com dados enviados em requisições POST ou PUT, frequentemente em formato JSON.

12. @Scheduled: Usada para marcar um método para ser executado em intervalos regulares. É extremamente útil para tarefas de rotina automatizadas, como limpeza de cache, atualizações periódicas ou tarefas de monitoramento.

13. @Transactional: Aplica-se a métodos e classes, indicando que o método ou todos os métodos da classe devem ser executados dentro de uma transação de banco de dados. É particularmente importante em operações que requerem consistência de dados.