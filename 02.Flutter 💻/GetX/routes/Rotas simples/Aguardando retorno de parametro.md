
//Aguardando parametro com a navegação normal (repare no await)
//Enquanto o usuario nao der o pop da proxima tela(AguardandoParams), ele vai ficar preso nesse //await

TextButton(
	onPressed: () async {
		final result = await Navigator.of(context).push(MaterialPageRoute(builder: (context) {
	builder: (context) {
		return const AguardandoParams()
	},
		print(result);
		}))
	}
)


//recebendo o parametro

class AguardandoParam extends StatelessWidget {
	const AguardandoParam({key? key}) : super(key: key);

	@Override
	Widget build(BuildContext context) {
	final paramNative = ModalRoute.of(context)?.settings.arguments ?? 'parametro nao enviado';
		

	return Scaffold(
		appBar: AppBar(
			title: const Text("retornando parametro"),
			body: TextButton(
	onPressed: ()  {
		Navigator.of(context).pop('Retornando parametro no flutter nativo');
	}
}

-------------------------------------------------------------------------------

//Aguarando o parametro (repare no await)
//Enquanto o usuario nao der o pop da proxima tela(AguardandoParams), ele vai ficar preso nesse //await
TextButton(
	onPressed: () async {
		final result = await Get.to(const AguardandoParam(),)
		print(result);
	}
)

//recebendo o parametro

class AguardandoParam extends StatelessWidget {
	const AguardandoParam({key? key}) : super(key: key);

	@Override
	Widget build(BuildContext context) {
		final paramGetX = Get.arguments ?? 'parametro nao enviado';

	return Scaffold(
		appBar: AppBar(
			title: const Text("retornando parametro"),
			body: TextButton(
	onPressed: ()  {
		Get.back(result: 'Retornando parametro no flutter nativo')
	}
)
		)
	)

	}
}
