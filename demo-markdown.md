<header><h1>Demo-Markdown</h1></header>
    <div id="container">
        <div id="presentacion">
            <h1>Bienvenido a mi presentación en <a href="https://markdown.es/" target="_blank">Markdown</a></h1>
            <blockquote><h2>En esta presentación veras un poco de codigo de los lenguajes que he ido aprendiendo a lo largo de 1º de DAW</h2></blockquote>
        </div>
<h2>java</h2>
        

    
    package ejercicio1;
    public enum DiaDeLaSemana {
	LU("Lunes", 1),
	MA("Martes", 2),
	MI("Miercoles", 3),
	JU("Jueves", 4),
	VI("Viernes", 5),
	SA("Sabado", 6),
	DO("Domingo", 7),;
	
	private String nombreCompleto;
	private int numeroDeDia;
	
	
	private DiaDeLaSemana(String nombreCompleto, int numeroDeDia) {
		this.nombreCompleto = nombreCompleto;
		this.numeroDeDia = numeroDeDia;
	}
	
	
	
	public String getNombreCompleto() {
		return nombreCompleto;
	}



	public int getNumeroDeDia() {
		return numeroDeDia;
	}



	public DiaDeLaSemana siguenteDia() {
		switch (this) {
		case LU: {
			return MA;
		}
		case MA: {
			return MI;
		}
		case MI: {
			return JU;
		}
		case JU: {
			return VI;
		}
		case VI: {
			return SA;
		}
		case SA: {
			return DO;
		}
		case DO: {
			return LU;
		}
		default:
			return null;
		}
	}
	
	public DiaDeLaSemana diaAnterior() {
		switch (this) {
		case DO: {
			return SA;
		}
		case SA: {
			return VI;
		}
		case VI: {
			return JU;
		}
		case JU: {
			return MI;
		}
		case MI: {
			return MA;
		}
		case MA: {
			return LU;
		}
		case LU: {
			return DO;
		}
		default:
			return null;
		}
	}
	
	@Override
	
	public String toString() {
		return String.format("Soy el dia %s y soy el numero %d de la semana", this.nombreCompleto, this.numeroDeDia);
	}
    }

<h2>html</h2>
            
            <div id="html" class="codigo">
                
            </div>
            <div id="sql" class="codigo">

            </div>
            <div id="JavaScript" class="codigo">

            </div>
        
