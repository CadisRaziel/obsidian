
//Enviando parametro com a navegação normal
Navigator.of(context).push(MaterialPageRoute(builder: (context) {
	builder: (context) {
		return const SendParams()
	},
	settings: RouteSettings(
		arguments: 'Parametro flutter nativo'
	)
}))

//recebendo o parametro

class SendParam extends StatelessWidget {
	const SendParam({key? key}) : super(key: key);

	@Override
	Widget build(BuildContext context) {
	final paramNative = ModalRoute.of(context)?.settings.arguments ?? 'parametro nao enviado';
		

	return Scaffold(
		appBar: AppBar(
			title: const Text("Recebendo parametro"),
			body: Center(child: Text(paramNative))
		)
	)

	}
}

-------------------------------------------------------------------------------

//Enviado parametro
Get.to(const SendParam(), arguments: "parametro pelo getX")

//recebendo o parametro

class SendParam extends StatelessWidget {
	const SendParam({key? key}) : super(key: key);

	@Override
	Widget build(BuildContext context) {
		final paramGetX = Get.arguments ?? 'parametro nao enviado';

	return Scaffold(
		appBar: AppBar(
			title: const Text("Recebendo parametro"),
			body: Center(child: Text(paramNative))
		)
	)

	}
}
