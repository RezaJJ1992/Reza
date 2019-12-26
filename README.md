Hello to all

First of all I am from Iran and I Cant Speak English Very Good sorry for this.

I made something like OpenFileDialog in Win.Form

and work correctly.

after for better User Interface I try to make it in WPF

I am use TreeView and other controls for made it in both platform(Winform,WPF)

in WPF I want to get text of Tree view Item For Compare,in winform i could do this by below code

private void Folder_FileTreeView_NodeMouseDoubleClick(object sender, TreeNodeMouseClickEventArgs e)
{

if(e.Node.Text=="Desktop")

{

\Do something

}

}

in Wpf I added text with Image next to each other by this method:

public object Node(string NodeIMGUri, string NodeText)
{

        Image IMG = new Image() { Source = new System.Windows.Media.Imaging.BitmapImage(new Uri(NodeIMGUri, UriKind.RelativeOrAbsolute)) };
        TextBlock Text = new TextBlock() { Text = NodeText };
        StackPanel CustomStackPanel = new StackPanel();
        TreeViewItem TVItem = new TreeViewItem();
        IMG.Height = 50;
        IMG.Width = 50;
        CustomStackPanel.Orientation = Orientation.Horizontal;
        CustomStackPanel.Children.Add(IMG);
        CustomStackPanel.Children.Add(Text);
        TVItem.Header = CustomStackPanel;
        return TVItem;
    }

But When in SelectedItemChange Event of Treeview try to get text of Item clicked(Or ItemChange)

i cant get text of Treeview Item

if help to me for compelete this Dll I can send it free to all programmer. this dll support most of language like germany france china hindi bengali indonesian persian japanese korean arabic portugues latin swede english

Thanks all
