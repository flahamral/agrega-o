# agrega-o
package ultraemojicombate;

/**
 *
 * @author Usuario
 */
public class UltraEmojiCombate {

      public static void main(String[] args) {
        // TODO code application logic here
        Lutador L[] = new Lutador[6];
         L[0] =  new Lutador("Pretty Boy","França",31,1.75f,
                 69.9f,11,2,1);       
         L[1] =  new Lutador("Putscript","Brasil",29,1.68f,
        57.8f,14,2,1);
           L[2] =  new Lutador("Snapshadow","EUA",35,1.65f,
        80.9f,12,2,1);
            L[3] =  new Lutador("Dead Code","Austrália",28,1.93f,
        81.6f,13,0,2);
             L[4] =  new Lutador("Ufucobol","Brasil",37,1.70f,
        119.3f,5,4,3);
              L[5] =  new Lutador("Nerdaard","EUA",30,1.81f,
        105.7f,12,2,4);
        
       L[3].status();
       L[4].apresentar();
       
          
    }
    
}


package ultraemojicombate;

/**
 *
 * @author Usuario
 */
public class Lutador {
     private String nome;
    private String nacionalidade;
    private int idade;
    private float altura;
    private float peso;
    private String categoria;
    private int vitorias,derrotas, empates;
    

    
    
 // metodos
    
    public void apresentar(){
        System.out.println("________________________________");
        System.out.println("Lutador: " + this.getNome());
        System.out.println("Nacionalidade: " + this.getNacionalidade());
        System.out.println("Idade : " + this.getIdade());
        System.out.println("Altura: " +this.getAltura());
        System.out.println("Peso: " +this.getPeso());
        System.out.println(" Tem: " + this.getVitorias() + " Vitorias ");
        System.out.println(this.getDerrotas() + " Derrotas ");
        System.out.println(" E "  + this.getEmpates() + " Empates ");
    } 
    public void status(){
        System.out.println("O nome dele é"+ this.getNome());
        System.out.println("é um peso "+ this.getCategoria());
        System.out.println(" Tem " + this.getVitorias() + " Vitorias " + this.getEmpates() + " Empates"+this.getDerrotas()+" Derrotas "); 
        
    }
    public void ganhar_luta(){
        setVitorias(getVitorias()+1);
    }
    public void perder_luta (){
        setDerrotas(getDerrotas()+1);
        
    }
    public void empatar_luta (){
        setEmpates(getEmpates()+1);
        
    }
     //

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getNacionalidade() {
        return nacionalidade;
    }

    public void setNacionalidade(String nacionalidade) {
        this.nacionalidade = nacionalidade;
    }

    public int getIdade() {
        return idade;
    }

    public void setIdade(int idade) {
        this.idade = idade;
    }

    public float getAltura() {
        return altura;
    }

    public void setAltura(float altura) {
        this.altura = altura;
    }

    public float getPeso() {
        return peso;
    }

    public void setPeso(float peso) {
        this.peso = peso;
        this.setCategoria();
    }

    public String getCategoria() {
        return categoria;
    }

      private void setCategoria() {
      if (this.peso< 52.2){
          this.categoria = "Invalido";        
    }else if(this.peso<=70.3){
        this.categoria = "Leve";
    }else if(this.peso <= 83.9){
        this.categoria = "Medio";
    }else if(this.peso <=120.2){
        this.categoria = "Pesado";
        
    }else{
        this.categoria ="Invalido";
    }
    }
    public int getVitorias() {
        return vitorias;
    }

    public void setVitorias(int vitorias) {
        this.vitorias = vitorias;
    }

    public int getDerrotas() {
        return derrotas;
    }

    public void setDerrotas(int derrotas) {
        this.derrotas = derrotas;
    }

    public int getEmpates() {
        return this.empates;
    }

    public void setEmpates(int empates) {
        this.empates = empates;
    }

    public Lutador(String nome, String nacionalidade, int idade, float altura, float peso, int vitorias, int derrotas, int empates) {
        this.nome = nome;
        this.nacionalidade = nacionalidade;
        this.idade = idade;
        this.altura = altura;
        this.setPeso(peso);
        this.vitorias = vitorias;
        this.derrotas = derrotas;
        this.empates = empates;
    }

   
    }


package ultraemojicombate;

public class Luta {
    private String desafiado;
    private String desafiante;
    private int round;
    private boolean aprovada;

public void marcar_luta (){
    
}    
public void lutar(){
    
}
    
}



