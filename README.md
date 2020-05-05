# Atividade-Avaliativa
public String efetuaLogin(HttpSession session) {

public String efetuaLogin(Usuario usuario, HttpSession session) {
    if(new JdbcUsuarioDao().existeUsuario(usuario)) {
        session.setAttribute("usuarioLogado", usuario);
        return "menu";
    } else {

<html>
          <body>
              <h2>Página de Login das Tarefas</h2>
              <form action="efetuaLogin" method="post">
                  Login: <input type="text" name="login" /> <br /> 
                  Senha: <input type="password" name="senha" /> <br />
                  <input type="submit" value="Entrar nas tarefas" /> 
              </form>
          </body>
      </html>
 @Gerenciar
      public class LoginController{

          @RequestMapping("loginForm")
          public String loginForm() {
              return "formulario-login";
          }
      }   
 
