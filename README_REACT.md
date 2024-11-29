Open VSCODE TERMINAL
// >  bracket mentions the code line i need to put on terminal or VSC

> npm create vite@latest //Development server - modern replacement to create react App 
> ? Project name: » my-react-app
//Select React and then java script later :
> cd my-react-app
> npm install
> npm run dev //to start development server
//then copy the local host link to see the development server in my case is
//run on browser --    http://localhost:5173/         
// No deleted the default function code in App.jsx and delete App.css, Now to create any new component Right click SRC and created Header.jsx
// create a function :
> fucntion Header() {
>
> <header>
  <h1>
    My Website
  </h1>
</header>
> }
> export default Header
//go to app Component to import header Component
//Now i make a other component Footer component 
>function Footer() {
return (

    <footer>
        <p>&copy; Your Website Name</p>
    </footer>
)
    
}
export default Footer

// Go to App.jsx and put footer and import it
//The whole code looks as follow : 
>
>'''React
import Header from './Header.jsx'
import Footer from './Footer.jsx'

function App() {
 return (
  <>
<Header/>
<Footer/>
</>
 );
}'''
//Here we get 2 component which is generally not allowed so i put empty angle bracket <></> called as fragments
fragments
//now making few more changes to Footer code you can enter javascript code in {}  in teturn statement trying to reflect 
//the current year automatically rel=flecting on website as: 

> 
'''React
function Footer() {
return (

    <footer>
        <p>&copy; {new Date().getFullYear()}Your Website Name</p>
    </footer>
)
    
}
export default Footer'''

