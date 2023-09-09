# TCP_Client_Meridian

<Window x:Class="Dizain.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:Dizain"
        mc:Ignorable="d"
        Title="TCP Client" Height="600" Width="700" WindowStyle="ThreeDBorderWindow" Background="White" FontWeight="Normal" ResizeMode="CanResizeWithGrip" FontSize="16">
    <Grid x:Name="MainRoot" Background="White">
        <Grid.RowDefinitions>
            <RowDefinition Height="1*"/>
            <RowDefinition Height="Auto"/>
        </Grid.RowDefinitions>

        <Grid Grid.Row="0">
            <Grid.ColumnDefinitions>
                <ColumnDefinition Width="1*"/>
                <ColumnDefinition Width="Auto"/>
            </Grid.ColumnDefinitions>

            <Grid  Grid.Column="0" Background='Red'>
                <Grid.RowDefinitions>
                    <RowDefinition Height="20"/>
                    <RowDefinition Height="*"/>
                </Grid.RowDefinitions>
                <TextBox Margin="5" Grid.Row="1"/>
                <TextBlock Text="Received/Senr data" FontSize="18" Width="160" Height="25" HorizontalAlignment="Left" Grid.Row="0" Margin="5 0 0 0"/>
            </Grid>

            <Grid  Grid.Column="1" Background='Green' Width="200">
                <Grid.RowDefinitions>
                    <RowDefinition Height="70"/>
                    <RowDefinition Height="50"/>
                    <RowDefinition Height="auto"/>
                </Grid.RowDefinitions>
                <Button Content="Ping" Height="30" Width="80" Margin="-10,-5,100,15" Grid.Row="1" />
                <Button Content="Connect" Height="30" Width="80" Margin="110,-5,10,15" Grid.Row="1" />
                <TextBox Text="192.169.1.1" Height="30" Width="130" Margin="5,15,65,5" Grid.Row="0"/>
                <TextBox Text="23" Height="30" Margin="148,15,10,5" Grid.Row="0"/>
                <TextBlock Text="Port" Height="20" Width="30" Margin="135 -35 10 10"/>
                <TextBlock Text="Module IP" Height="20" Width="80" Margin="-100 -35 10 10"/>



            </Grid>



        </Grid>

        <Grid Grid.Row="1">
            <Grid Background="Yellow" Height="150">
                <Grid.RowDefinitions>
                    <RowDefinition/>
                    <RowDefinition/>
                    <RowDefinition/>
                </Grid.RowDefinitions>
                <Grid.ColumnDefinitions>
                    <ColumnDefinition Width="5*"/>
                    <ColumnDefinition Width="auto"/>
                    <ColumnDefinition Width="auto"/>
                </Grid.ColumnDefinitions>

                <TextBox Height="30" Width="auto" Grid.Column="0" Grid.Row="0"  Margin="10"/>
                <TextBox Height="30" Width="auto" Grid.Column="0" Grid.Row="1"  Margin="10"/>
                <TextBox Height="30" Width="auto" Grid.Column="0" Grid.Row="2"  Margin="10"/>
                <CheckBox Content="HEX" Grid.Column="1" Grid.Row="0" Width="50" Margin="10"/>
                <CheckBox Content="HEX" Grid.Column="1" Grid.Row="1" Width="50" Margin="10"/>
                <CheckBox Content="HEX" Grid.Column="1" Grid.Row="2" Width="50" Margin="10"/>
                <Button Content="Send" Height="30" Width="90" Grid.Column="2" Grid.Row="1" Margin="5" />
                <Button Content="Send" Height="30" Width="90" Grid.Column="2" Grid.Row="2" Margin="5" />
                <Button Content="Send" Height="30" Width="90" Grid.Column="2" Grid.Row="0"  />
            </Grid>
        </Grid>






    </Grid>
</Window>
