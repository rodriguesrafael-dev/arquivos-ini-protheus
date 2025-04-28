# arquivos-ini-protheus
Configuracao dos principais arquivos .ini do ERP Protheus

# banco de dados
    encoding: WIN1252
    locale provider: libc
    collation: C
    Character type: C

# servicos
    .00.TOTVS|LicenseServerVirtual      Servidor de Licencas
    .01.TOTVS|AppServer12_Broker        Balanceamento de Carga
    .02.TOTVS|DBAccess_TopConnect       Conexao Banco de Dados
    .03.TOTVS|AppServer12               Servidor de Aplicacao
    .04.TOTVS|AppServer12_REST          Servidor WebService

# broker (-i = install) (-d = debug)
    -i -balance_smart_client_desktop 	
    -d -balance_smart_client_desktop 	

# smartclient desktop
    -p=SIGAMDI -e=PROTHEUS -c=TCP -M