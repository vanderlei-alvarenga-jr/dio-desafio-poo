::: mermaid
---
title: Diagrama de Classe iPhone
---
classDiagram
    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet

    class iPhone{
        <<instance>>
    }

    class ReprodutorMusical{
        +listarPlaylists()
        +listarArtistas()
        +listarTodasMusicas()
        +listarVideos()
        +apresentarMaisOpcoes()
        +listarAlbuns(Artista)
        +listarMusicas(Artista, Album)
        +reproduzirMusica(Musica)
        +mostrarControlesMusica(Musica)
        +pausarReproducaoMusica(Musica)
        +pularInicioMusica(Musica)
        +pularMusicaParaTempo(Tempo, Musica)
        +pularProximaMusica(ListaReproducaoMusica, PosicaoMusicaAtual)
        +pularMusicaAnterior(ListaReproducaoMusica, PosicaoMusicaAtual)
        +mostrarListaReproducaoMusica(ListaReproducaoMusica)
        +mostrarControleVolume()
        +regularVolume(PorcentagemVolume)
        +avaliarAlbum(Avaliacao)
        +apresentarCoverFlow()
        +listarAlbuns()
        +listarAudiobooks()
        +listarCompilacoes()
        +listarPodcasts()
        +reproduzirVideo(Video)
        +mostrarControlesVideo(Video)
        +pausarReproducaoVideo(Video)
        +pularInicioVideo(Video)
        +pularVideoParaTempo(Tempo, Video)
        +pularProximaVideo(ListaReproducaoVideo, PosicaoVideoAtual)
        +pularVideoAnterior(ListaReproducaoVideo, PosicaoVideoAtual)
        +alternarModoFullScreen(Video)
        +voltarTelaAnterior()
    }
    class AparelhoTelefonico{
        +sincronizarContatos()
        +listarContatos()
        +mostrarHistoricoLigacoes(LigacoesRecebidas, LigacoesEfetuadas)
        +adicionarContato(NumeroContato, NomeContato, DadosOpcionais)
        +favoritarContato(Contato)
        +ordenarListaContatosFavoritos(ListaContatosFavoritos)
        +removerContatoFavoritos(ListaContatosFavoritos)
        +detalharDadosContato(Contato)
        +mostrarLigacaoChamando()
        +ligar(NumeroDigitado)
        +desativarMicrofoneLigacao(LigacaoAtiva)
        +ativarMicrofoneLigacao(LigacaoAtiva)
        +ativarVivaVozLigacao(LigacaoAtiva)
        +desativarVivaVozLigacao(LigacaoAtiva)
        +ajustarVolumeLigacao(LigacaoAtiva, PorcentagemVolume)
        +atenderSegundaLigacaoEColocarPrimeiraLigacaoEmEspera(LigacaoAtiva, LigacaoRecebida)
        +voltarPrimeiraLigacaoEColocarSegundaLigacaoEmEspera(LigacaoAtiva, LigacaoEmEspera)
        +atenderSegundaLigacaoEEncerrarPrimeiraLigacao(LigacaoAtiva, LigacaoRecebida)
        +encerrarSegundaLigacaoEVoltarParaPrimeiraLigacao(LigacaoAtiva, LigacaoEmEspera)
        +colocarPrimeiraESegundaLigacoesEmConferencia(LigacaoAtiva, LigacaoEmEspera)
        +voltarChamadaPrivadaNaConferencia(ListaLigacoesConferencia, LigacaoSelecionadaPrivada)
        +encerrarLigacao(LigacaoAtiva)
        +receberLigacao(LigacaoChamando)
        +rejeitarLigacao(LigacaoChamando)
        +silenciarLigacao(LigacaoChamando)
        +redirecionarParaCaixaPostal(LigacaoChamando)
        +listarMensagensCaixaPostal()
        +reproduzirMensagemCaixaPostal(MensagemSelecionada)
    }
    class NavegadorInternet{
        +carregarURL(urlDigitada)
        +aumentarZoom(posicaoPagina)
        +diminuirZoom(posicaoPagina)
        +removerZoom()
        +selecionarLinkPagina()
        +carregarLinkEmNovaAba()
        +voltarPaginaAnterior()
        +avancarPaginaPosterior()
        +listarLinksFavoritos()
        +adicionarLinkListaFavoritos(ListaLinksFavoritos)
        +removerLinkListaFavoritos(ListaLinksFavoritos, LinkFavoritado)
    }
:::