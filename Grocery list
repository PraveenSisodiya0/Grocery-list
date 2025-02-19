grocery_list = []

def show_menu():
    print("\n===== Grocery List =====")
    print("1. Add an item")
    print("2. Remove an item")
    print("3. See the list")
    print("4. Clear the list")
    print("5. Exit")

while True:
    show_menu()
    choice = input("Choose an option (1-5): ")

    if choice == "1":
        item = input("What do you want to add? ").strip()
        if item:
            grocery_list.append(item)
            print(f"Added '{item}' to your list.")
        else:
            print("Please enter something.")

    elif choice == "2":
        if grocery_list:
            item = input("What do you want to remove? ").strip()
            if item in grocery_list:
                grocery_list.remove(item)
                print(f"Removed '{item}' from your list.")
            else:
                print(f"'{item}' is not in the list.")
        else:
            print("The list is empty.")

    elif choice == "3":
        if grocery_list:
            print("\nYour Grocery List:")
            for i, item in enumerate(grocery_list, start=1):
                print(f"{i}. {item}")
        else:
            print("Your list is empty.")

    elif choice == "4":
        confirm = input("Are you sure you want to clear the list? (yes/no): ").strip().lower()
        if confirm == "yes":
            grocery_list.clear()
            print("The list is now empty.")
        else:
            print("List was not cleared.")

    elif choice == "5":
        print("Goodbye!")
        break

    else:
        print("Please enter a number from 1 to 5.")
