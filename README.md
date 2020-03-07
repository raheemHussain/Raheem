# Raheem

How I did the task?

I first started by using MVC which I am quite familar with. I inserted a database to get all the cars, having the an ID for each indiviudual car.
At the end column you will see a column for admin, if it is true then the admin will be able to add a car/ edit a car or delete a car.

The login page will expect a login for the user and once logged in then you will be able to display the car. If the user is unsuccessful it 
will display a message for the user indicating that it was unsuccessful and the username and the password are correct then it will be
successful.

Admin User,
test
test

If you would like to see this feature being used then please login as the admin and the details are provided above

You will also be able to see the register a user from the login page by simply selecting register new user.

I have tried my best to use React however I have not been able to get my head around it, I have been looking at tutorial to see how it works.
You will be able to see in the scripts folder that I have added the package for React however it does not seem to connect with my view.

import MuiThemeProvider from 'material-ui/styles/MuiThemeProvider';
import AppBar from 'material-ui/AppBar';
import RaisedButton from 'material-ui/RaisedButton';
import TextField from 'material-ui/TextField';
class Login extends Component {
    constructor(props) {
        super(props);
        this.state = {
            username: '',
            password: ''
        }
    }
    render() {
        return (
            <div>
                <MuiThemeProvider>
                    <div>
                        <AppBar
                            title="Login"
                        />
                        <TextField
                            hintText="Enter your Username"
                            floatingLabelText="Username"
                            onChange={(event, newValue) => this.setState({ username: newValue })}
                        />
                        <br />
                        <TextField
                            type="password"
                            hintText="Enter your Password"
                            floatingLabelText="Password"
                            onChange={(event, newValue) => this.setState({ password: newValue })}
                        />
                        <br />
                        <RaisedButton label="Submit" primary={true} style={style} onClick={(event) => this.handleClick(event)} />
                    </div>
                </MuiThemeProvider>
            </div>
        );
    }
}
const style = {
    margin: 15,
};
export default Login;

Here is an example of what I wanted to include but could not seem to find where it goes.

I hope under your guidelines I would be able to add the feature as well.
