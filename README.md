# Teste Caixa Branca Etapa 3

A técnica de caixa-branca atenta mais ao funcionamento interno do sistema. Também conhecido como
teste estrutural ou teste de caixa de vidro tem como foco testes que são aplicados nas estruturas internas
dos sistemas. Ao contrário do que ocorre nos testes de caixa-preta, a aplicação dos testes de caixa-branca
fornece resultados que possibilitam uma análise diretamente relacionada ao código-fonte do sistema
## Codigo Teste Caixa Branca 
```
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.Statement;

public class User {
    /*  Método para estabelecer uma conexão com o banco de dados */
    public Connection conectarBD(){ 
        Connection conn = null;
        
        try{
            /* <codigo-fonte> Carregando o driver do MySQL */
            Class.forName("com.mysql.Driver.Manager").newInstance(); // NO 1
            String url = "jdbc:mysql://127.0.0.1/test?user=lopes&password=123"; // NO 2
            conn = DriverManager.getConnection(url); // NO 3
        } catch (Exception e) { 
            /* Tratamento com as exceções */
        }  
        return conn;
    }
    
    /* Variáveis de instância */
    public String nome = ""; 
    public boolean result = false; 

    /* Verificar se o usuário existe no banco de dados */
    public boolean verificarUsuario(String login, String senha){  
        String sql = ""; 
        Connection conn = conectarBD(); 
        
        /* INTRODUÇÃO SQL */
        sql += "select nome from usuarios "; 
        sql += "where login = " + "'" + login + "'"; 
        sql += " and senha = " + "'" + senha + "';"; // NO 5
        
        try { 
            Statement st =  conn.createStatement(); //NO 6
            ResultSet rs = st.executeQuery(sql); // NO 7 
            if(rs.next()){ // NO 8
                result = true; //NO 9 
                nome = rs.getString("nome"); // NO 10
            } 
        } catch (Exception e) {
           
        }
        return result; // NO 11
    } 
}



# O que esta feito no codigo acima ? 
No código apresentado, notamos uma abordagem de documentação que abrange classes, métodos e variáveis. Além disso, são identificadas as etapas críticas no fluxo do código marcando os seus Nó . 

# Tecnologia 
Linguagem de Programação Java 

# IDE 
APACHE NETBEANS IDE 17

# ULTIMA ATUALIZAÇÃO 17/10/2023





