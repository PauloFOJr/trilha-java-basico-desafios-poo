
classDiagram
direction TB
    class IPhone {
    }

    class ReprodutorMusical {
	    +tocar() void
	    +pausar() void
	    +selecionarMusica() String
    } 

    class AparelhoTelefonico {
	    +ligar() String
	    +atender() void
	    +iniciarCorreioVoz() void
    }

    class NavegadorInternet {
	    +exibirPagina() String
	    +adicionarNovaAba() void
	    +atualizarPagina() void
    }

	<<interface>> ReprodutorMusical
	<<interface>> AparelhoTelefonico
	<<interface>> NavegadorInternet

    IPhone --> ReprodutorMusical
    IPhone --> AparelhoTelefonico
    IPhone --> NavegadorInternet
