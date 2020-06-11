#include <iostream>
using namespace std;
char matrix[3][3] = { '1', '2', '3', '4', '5', '6', '7', '8', '9' };
char player = 'X';
int chances;
void Draw()
{
    system("clear");
    cout << "*=====================*" << endl;
    cout << "|                     |" << endl;
    cout << "|  Tic Tac Toe V.1.1  |"<< endl;
    cout << "|                     |" << endl;
    cout << "*=====================*" << endl;
    cout << endl;
    cout << endl;

    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            cout << "    " << matrix[i][j] << "  ";
        }
        cout << endl;
    }
}
void Input()
{
    int input;
    cout << endl;
    cout << endl;
    cout << "It's " << player << " turn. " <<"Press the number you want : ";
    cin >> input;
 
    if (input == 1)
    {
        if (matrix[0][0] == '1')
            matrix[0][0] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 2)
    {
        if (matrix[0][1] == '2')
            matrix[0][1] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 3)
    {
        if (matrix[0][2] == '3')
            matrix[0][2] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 4)
    {
        if (matrix[1][0] == '4')
            matrix[1][0] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 5)
    {
        if (matrix[1][1] == '5')
            matrix[1][1] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 6)
    {
        if (matrix[1][2] == '6')
            matrix[1][2] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 7)
    {
        if (matrix[2][0] == '7')
            matrix[2][0] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 8)
    {
        if (matrix[2][1] == '8')
            matrix[2][1] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
    else if (input == 9)
    {
        if (matrix[2][2] == '9')
            matrix[2][2] = player;
        else
        {
            cout << "Already in use try again!" << endl;
            Input();
        }
    }
     
}
void TogglePlayer()
{
    if (player == 'X')
        player = 'O';
    else
        player = 'X';
}
char Win()
{
    //first player
    if (matrix[0][0] == 'X' && matrix[0][1] == 'X' && matrix[0][2] == 'X')
        return 'X';
    if (matrix[1][0] == 'X' && matrix[1][1] == 'X' && matrix[1][2] == 'X')
        return 'X';
    if (matrix[2][0] == 'X' && matrix[2][1] == 'X' && matrix[2][2] == 'X')
        return 'X';
 
    if (matrix[0][0] == 'X' && matrix[1][0] == 'X' && matrix[2][0] == 'X')
        return 'X';
    if (matrix[0][1] == 'X' && matrix[1][1] == 'X' && matrix[2][1] == 'X')
        return 'X';
    if (matrix[0][2] == 'X' && matrix[1][2] == 'X' && matrix[2][2] == 'X')
        return 'X';
 
    if (matrix[0][0] == 'X' && matrix[1][1] == 'X' && matrix[2][2] == 'X')
        return 'X';
    if (matrix[2][0] == 'X' && matrix[1][1] == 'X' && matrix[0][2] == 'X')
        return 'X';
 
    //second player
    if (matrix[0][0] == 'O' && matrix[0][1] == 'O' && matrix[0][2] == 'O')
        return 'O';
    if (matrix[1][0] == 'O' && matrix[1][1] == 'O' && matrix[1][2] == 'O')
        return 'O';
    if (matrix[2][0] == 'O' && matrix[2][1] == 'O' && matrix[2][2] == 'O')
        return 'O';
 
    if (matrix[0][0] == 'O' && matrix[1][0] == 'O' && matrix[2][0] == 'O')
        return 'O';
    if (matrix[0][1] == 'O' && matrix[1][1] == 'O' && matrix[2][1] == 'O')
        return 'O';
    if (matrix[0][2] == 'O' && matrix[1][2] == 'O' && matrix[2][2] == 'O')
        return 'O';
 
    if (matrix[0][0] == 'O' && matrix[1][1] == 'O' && matrix[2][2] == 'O')
        return 'O';
    if (matrix[2][0] == 'O' && matrix[1][1] == 'O' && matrix[0][2] == 'O')
        return 'O';
 
    return '/';
}
int main()
{
    chances = 0;
    Draw();
    while (1)
    {
        chances++;
        Input();
        Draw();
        if (Win() == 'X')
        {
            cout << endl;
            cout << endl;
            cout << "      X wins!" << endl;
            cout << endl;
            cout << endl;
            break;
        }
        else if (Win() == 'O')
        {
            cout << endl;
            cout << endl;
            cout << "      O wins!" << endl;
            cout << endl;
            cout << endl;
            break;
        }
        else if (Win() == '/' && chances == 9)
        {
            cout << endl;
            cout << endl;
            cout << "     It's a draw!" << endl;
            cout << endl;
            cout << endl;
            break;
        }
        TogglePlayer();
    }
    return 0;
}
