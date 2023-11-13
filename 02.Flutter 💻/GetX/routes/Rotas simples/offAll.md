


//Excluir todas as telas da pilha
• Get.offAll(const PageWidget1); o get não precisa de rota nomeada ou parametro  

• Navigator.of(context).popAndRemoveUntil (pra usa essa navegação ela tem que ter um nome(seria rota nomeada), quando nao tiver rotaNomeada usar arguments)
Ele exclui todas as telas da pilha

-----------------------------------------------------------------------------

//Gerenciar a exclusão de todas as telas até uma determinada pagina
• Get.offAll(const PageWidget1); o get não precisa de rota pois ele mesmo cria o nome(quando voce cria a pagina ele pega o nome dela como rota nomeada) porém no get nós utilizamos o 'predicate: ModalRoute.withName('/PageWidget3'),' 

• Navigator.of(context).popAndRemoveUntil passando a propriedade ModalRoute.withName('nameRoute'), ele só vai excluir(volte ou va) as telas até a tela que voce passar no 'nameRoute'
