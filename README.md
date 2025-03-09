<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             x:Class="PopcornApp.MainPage">

    <Grid RowDefinitions="Auto, *, Auto" Padding="10">

        <!-- Navigation Bar -->
        <StackLayout Orientation="Horizontal" BackgroundColor="Purple" Padding="20" Grid.Row="0">
            <Image Source="popss.jpg" WidthRequest="30" HeightRequest="30" />
            <Label Text="Kernelicious" FontSize="20" TextColor="White" VerticalOptions="Center" Margin="10,0,0,0" />
        </StackLayout>

        <!-- Popcorn Selection -->
        <Grid Grid.Row="1" ColumnDefinitions="*,*" RowDefinitions="*,*" Padding="10">

            <!-- Cheese -->
            <Border Grid.Row="0" Grid.Column="0" Stroke="White" StrokeShape="RoundRectangle 10" Padding="10">
                <Grid>
                    <Image Source="popss.jpg" Aspect="Fill" Opacity="0.5"/>
                    <!-- Lower opacity -->
                    <StackLayout Padding="10">  
                        <Label Text="Cheese" FontSize="18" TextColor="White"/>
                        <CheckBox x:Name="cheeseCheckBox"/>
                    </StackLayout>
                </Grid>
            </Border>

            <!-- Sour -->
            <Border Grid.Row="0" Grid.Column="1" Stroke="White" StrokeShape="RoundRectangle 10" Padding="10">
                <Grid>
                    <Image Source="popss.jpg" Aspect="Fill" Opacity="0.5"/>
                    <StackLayout Padding="10">
                        <Label Text="Sour and Cream" FontSize="18" TextColor="White"/>
                        <CheckBox x:Name="sourCheckBox"/>
                    </StackLayout>
                </Grid>
            </Border>

            <!-- BBQ -->
            <Border Grid.Row="1" Grid.Column="0" Stroke="White" StrokeShape="RoundRectangle 10" Padding="10">
                <Grid>
                    <Image Source="popss.jpg" Aspect="Fill" Opacity="0.5"/>
                    <StackLayout Padding="10">
                        <Label Text="BBQ" FontSize="18" TextColor="White"/>
                        <CheckBox x:Name="bbqCheckBox"/>
                    </StackLayout>
                </Grid>
            </Border>

            <!-- Spicy BBQ -->
            <Border Grid.Row="1" Grid.Column="1" Stroke="White" StrokeShape="RoundRectangle 10" Padding="10">
                <Grid>
                    <Image Source="popss.jpg" Aspect="Fill" Opacity="0.5"/>
                    <StackLayout Padding="10">
                        <Label Text="Spicy BBQ" FontSize="18" TextColor="White"/>
                        <CheckBox x:Name="spicyBbqCheckBox"/>
                    </StackLayout>
                </Grid>
            </Border>

        </Grid>

        <!-- Order Button -->
        <Button Text="Order" Grid.Row="2" BackgroundColor="Purple" TextColor="White" 
                FontSize="18" CornerRadius="10" WidthRequest="200" HeightRequest="50"
                HorizontalOptions="Center" VerticalOptions="End" />

    </Grid>
</ContentPage>
