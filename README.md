from django.db import models, migrations




class Migration(migrations.Migration):

    initial = True

    dependencies = [
    ]

    operations = [
        migrations.CreateModel(
            name="Asvertisement",
            fields=[
                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
                ("title", models.CharField(max_length=100, verbose_name="Название")),
                ("description", models.TextField(verbose_name="Описание")),
                ("price", models.DecimalField(decimal_places=2, max_digits=10, verbose_name="Цена")),
                ("auctiion", models.BooleanField(default=False, verbose_name="Торг")),
                ("created_at", models.DateTimeField(auto_now_add=True, verbose_name="Дата публикации")),
                ("updated_at", models.DateTimeField(auto_now=True, verbose_name="Дата рекодирования"))
            ],
        ),
    ]
