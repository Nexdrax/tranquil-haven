#include <iostream>
#include <string>

using namespace std;

void displayWelcomeMessage() {
    cout << "Welcome to Tranquil Haven!" << endl;
    cout << "A place of peace and serenity." << endl << endl;
}

void displayGardenDescription() {
    cout << "You are in a beautiful garden filled with colorful flowers," << endl;
    cout << "chirping birds, and a gentle breeze rustling the leaves." << endl;
    cout << "You can explore different parts of the garden to find your own" << endl;
    cout << "spot of tranquility." << endl << endl;
}

void exploreGarden() {
    int choice;
    do {
        cout << "Where would you like to go?" << endl;
        cout << "1. Flower Meadow" << endl;
        cout << "2. Tranquil Pond" << endl;
        cout << "3. Shady Grove" << endl;
        cout << "4. Exit" << endl;
        cout << "Enter your choice: ";
        cin >> choice;
        cout << endl;

        switch(choice) {
            case 1:
                cout << "You walk into the flower meadow. The fragrance of flowers fills the air." << endl << endl;
                break;
            case 2:
                cout << "You sit by the tranquil pond. The sound of water soothes your soul." << endl << endl;
                break;
            case 3:
                cout << "You find a shady grove. The cool shade provides relief from the sun." << endl << endl;
                break;
            case 4:
                cout << "Thank you for visiting Tranquil Haven. Come back soon!" << endl << endl;
                break;
            default:
                cout << "Invalid choice. Please try again." << endl << endl;
        }
    } while (choice != 4);
}

int main() {
    displayWelcomeMessage();
    displayGardenDescription();
    exploreGarden();
    return 0;
}
