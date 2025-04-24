# Projeto-Forms1-FrmMenu
Criação de Formularios Menu do Windows

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ProjetoForms1
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
            //evento do relógio
            lblHora.Text = DateTime.Now.ToLongTimeString();
        }

private void btnClientes_Click(object sender, EventArgs e)
        {
            FrmClientes cli=new FrmClientes();
            cli.ShowDialog();
        }

private void btnProdutos_Click(object sender, EventArgs e)
        {
            FrmProdutos prod=new FrmProdutos();
            prod.ShowDialog();
        }

private void btnMarcas_Click(object sender, EventArgs e)
        {
            FrmMarcas marca=new FrmMarcas();
            marca.ShowDialog();
        }

private void btnFornecedores_Click(object sender, EventArgs e)
        {
            FrmFornecedores fornecedor=new FrmFornecedores();
            fornecedor.ShowDialog();
        }

private void btnVendas_Click(object sender, EventArgs e)
        {
            FrmVendas vendas=new FrmVendas();  
            vendas.ShowDialog();
        }

private void pictureBox1_Click(object sender, EventArgs e)
        {

}

private void FrmMenu_Load(object sender, EventArgs e)
        {

}
}
}
