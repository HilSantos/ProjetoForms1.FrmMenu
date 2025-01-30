# Projeto-Forms-2025
Criação de Formularios do Windows

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ProjetoForms2025
{
    public partial class FrmMenu : Form
    {
        public FrmMenu()
        {
            InitializeComponent();
            lblData.Text=DateTime.Now.ToLongDateString();
        }

  private void timer1_Tick(object sender, EventArgs e)
        {
            //evento do relogio
            lblHora.Text = DateTime.Now.ToLongTimeString();
        }

  private void btnClientes_Click(object sender, EventArgs e)
        {
            FrmClientes clientes = new FrmClientes();
            clientes.ShowDialog();
        }

  private void btnProdutos_Click(object sender, EventArgs e)
        {
            Produtos produtos = new Produtos();
            produtos.ShowDialog();
        }

  private void btnMarcas_Click(object sender, EventArgs e)
        {
            Marcas marcas = new Marcas();
            marcas.ShowDialog();
        }

  private void btnFornecedores_Click(object sender, EventArgs e)
        {
            Fornecedores fornecedores = new Fornecedores();
            fornecedores.ShowDialog();
        }

  private void btnVendas_Click(object sender, EventArgs e)
        {
            Vendas vendas = new Vendas();
            vendas.ShowDialog();
        }
    }
}
