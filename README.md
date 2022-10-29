using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace sales_Computing_Sysem
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void tb_hammers_qty_Leave(object sender, EventArgs e)
        {
            int hammer_qty;
            double hammers_line_total;
            hammer_qty = int.Parse(tb_hammers_qty.Text);
            hammers_line_total = hammer_qty * double.Parse(lb_hammers_price.Text);
            lb_line_total_hammers.Text = hammers_line_total.ToString();
            lb_total.Text = (Double.Parse(lb_line_total_hammers.Text) + Double.Parse(lb_line_total_screwdriver.Text) + Double.Parse(lb_line_total_chisels.Text) + Double.Parse(lb_line_total_chainsaw.Text) + Double.Parse(lb_line_total_wireless.Text)).ToString();


        }

        private void textBox2_Leave(object sender, EventArgs e)
        {

        }

        private void tb_screwdriver_qty_Leave(object sender, EventArgs e)
        {
            int screwdriver_qty;
            double screwdriver_line_total;
            screwdriver_qty = int.Parse(tb_screwdriver_qty.Text);
            screwdriver_line_total = screwdriver_qty * double.Parse(lb_screwdriver_price.Text);
            lb_line_total_screwdriver.Text = screwdriver_line_total.ToString();
            lb_total.Text = (Double.Parse(lb_line_total_hammers.Text) + Double.Parse(lb_line_total_screwdriver.Text) + Double.Parse(lb_line_total_chisels.Text) + Double.Parse(lb_line_total_chainsaw.Text) + Double.Parse(lb_line_total_wireless.Text)).ToString();

        }

        private void tb_chisels_qty_Leave(object sender, EventArgs e)
        {
            int chisels_qty;
            double chisels_line_total;
            chisels_qty = int.Parse(tb_chisels_qty.Text);
            chisels_line_total = chisels_qty * double.Parse(lb_chisels_price.Text);
            lb_line_total_chisels.Text = chisels_line_total.ToString();
            lb_total.Text = (Double.Parse(lb_line_total_hammers.Text) + Double.Parse(lb_line_total_screwdriver.Text) + Double.Parse(lb_line_total_chisels.Text) + Double.Parse(lb_line_total_chainsaw.Text) + Double.Parse(lb_line_total_wireless.Text)).ToString();

        }

        private void tb_chainsaw_qty_Leave(object sender, EventArgs e)
        {
            int chainsaw_qty;
            double chainsaw_line_total;
            chainsaw_qty = int.Parse(tb_chainsaw_qty.Text);
            chainsaw_line_total = chainsaw_qty * double.Parse(lb_chainsaw_price.Text);
            lb_line_total_chainsaw.Text = chainsaw_line_total.ToString();
            lb_total.Text = (Double.Parse(lb_line_total_hammers.Text) + Double.Parse(lb_line_total_screwdriver.Text) + Double.Parse(lb_line_total_chisels.Text) + Double.Parse(lb_line_total_chainsaw.Text) + Double.Parse(lb_line_total_wireless.Text)).ToString();


        }

        private void tb_wireless_qty_Leave(object sender, EventArgs e)
        {
            int wireless_qty;
            double wireless_line_total;
            wireless_qty = int.Parse(tb_wireless_qty.Text);
            wireless_line_total = wireless_qty * double.Parse(lb_wireless_price.Text);
            lb_line_total_wireless.Text = wireless_line_total.ToString();
            lb_total.Text = (Double.Parse(lb_line_total_hammers.Text) + Double.Parse(lb_line_total_screwdriver.Text) + Double.Parse(lb_line_total_chisels.Text) + Double.Parse(lb_line_total_chainsaw.Text) + Double.Parse(lb_line_total_wireless.Text)).ToString();



        }
    }
}
